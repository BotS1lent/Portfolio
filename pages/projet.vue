<template>
    <div class="container mx-auto p-4">
        <h1 class="text-3xl font-bold mb-4">Mes Projets</h1>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
            <div v-for="project in projects" :key="project.id" class="rounded-lg shadow-md p-4">
                <img :src="project.image" alt="Project Image" class="w-full h-48 object-cover rounded-md mb-4">
                <h2 class="text-xl font-semibold">{{ project.title }}</h2>
                <p class="text-gray-600">{{ project.description }}</p>
                <div class="mt-4">
                    <NuxtLink to="project.github" target="_blank" class="text-blue-500 hover:underline">Voir le code
                    </NuxtLink>
                    <span v-if="project.demo" class="mx-2">•</span>
                    <NuxtLink v-if="project.demo" to="project.demo" target="_blank"
                        class="text-blue-500 hover:underline">
                        Voir la démo
                    </NuxtLink>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            projects: [
                {
                    id: 1,
                    title: 'Portfolio',
                    description: 'Et oui ! Première expérience en front-end, fait en Vue avec Nuxt 3 et Tailwind CSS.',
                    image: 'portfolio.png',
                    github: 'https://github.com/BotS1lent/Portfolio',
                    demo: '/'
                },
                {
                    id: 2,
                    title: 'Glados/Jigot',
                    description: 'Projet d\'Epitech, où on devait créer notre propre langage de programmation en Haskell.',
                    image: 'glados.svg',
                    github: 'https://github.com/BotS1lent/Glados',
                    demo: null,
                }, {
                    id: 3,
                    title: 'Projet 3',
                    description: 'Description du projet 3.',
                    image: 'url-de-limage-1',
                    github: 'https://github.com/user/project1',
                    demo: 'https://demo.project1.com'
                },
                {
                    id: 4,
                    title: 'Projet 4,',
                    description: 'Description du projet 4,.',
                    image: 'url-de-limage-1',
                    github: 'https://github.com/user/project1',
                    demo: 'https://demo.project1.com'
                },
                // Ajoutez d'autres projets ici
            ]
        }
    }
}
</script>