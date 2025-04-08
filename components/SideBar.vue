<template>
    <nav class="w-64 bg-stone-800 text-white h-full flex flex-col">
        <div class="flex-grow">
            <div class="flex items-center justify-center h-20">
                <NuxtLink to="/">
                    <h1 class="text-[1.75em] font-bold">Tom Laumonier</h1>
                </NuxtLink>
            </div>
            <ul class="flex flex-col">
                <li class="mb-6">
                    <NuxtLink to="/" class="flex items-center gap-8 hover:bg-orange-700 w-full p-2">
                        <Icon name="mdi:home-outline" style="color: white" size="3em" />
                        <span class="w-full text-left text-xl">Accueil</span>
                    </NuxtLink>
                </li>
                <li class="mb-6">
                    <NuxtLink to="projet" class="flex items-center gap-8 hover:bg-orange-700 w-full p-2">
                        <Icon name="mdi:application-brackets-outline" style="color: white" size="3em" />
                        <span class="w-full text-left text-xl">Projets</span>
                    </NuxtLink>
                </li>
                <li class="mb-6">
                    <NuxtLink to="about" class="flex items-center gap-8 hover:bg-orange-700 w-full p-2">
                        <Icon name="mdi:information" style="color: white" size="3em" />
                        <span class="w-full text-left text-xl">À propos</span>
                    </NuxtLink>
                </li>
                <li>
                    <NuxtLink to="contact" class="flex items-center gap-8 hover:bg-orange-700 w-full p-2">
                        <Icon name="mdi:account-circle" style="color: white" size="3em" />
                        <span class="w-full text-left text-xl">Contact</span>
                    </NuxtLink>
                </li>
            </ul>
        </div>
        <div class="flex justify-center gap-4 p-4">
            <NuxtLink to="https://www.linkedin.com/in/tom-laumonier-78b1301b7/" target="_blank"
                class="rounded hover:bg-orange-700">
                <Icon name="mdi:linkedin" style="color: white" size="3em" />
            </NuxtLink>
            <NuxtLink to="https://github.com/BotS1lent" target="_blank" class="rounded hover:bg-orange-700">
                <Icon name="mdi:github" style="color: white" size="3em" />
            </NuxtLink>
        </div>
    </nav>
</template>

<script>
export default {
    name: 'SidebarLayout',
};
</script>