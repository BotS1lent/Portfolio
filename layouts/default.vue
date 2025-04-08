<template>
    <div class="flex h-screen">
        <SideBar class="fixed inset-y-0 left-0 w-64" />
        <main class="ml-64 flex-grow bg-gray-100 overflow-y-auto">
            <slot />
        </main>
    </div>
</template>

<style scoped>
/* Ajoutez des styles spécifiques ici si nécessaire */
</style>
