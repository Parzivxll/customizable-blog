<template>
    <section class="flex justify-between mb-4">
        <div class="w-[512px]">
            <h3 class="text-5xl mb-4 font-bold">
                {{ name }}
            </h3>
            <p class="text-lg">
                {{ description }}
            </p>
        </div>
        <div class="relative w-64 h-64 p-3 bg-c2 flex items-center justify-center rounded-3xl">
            <img class="rounded-3xl h-full w-full" :src="profilePhoto" alt="Profile Photo" />
            <div class="absolute bottom-0 translate-y-1/2 bg-c2 w-48 rounded-3xl h-16 flex items-center justify-center">
                <span class="text-xl font-medium">{{ tag }}</span>
            </div>
        </div>
    </section>
    <h3 class="text-2xl font-medium">I can do</h3>
    <section class="flex mt-2 mb-16">
        <h1 class="text-8xl cursor-pointer nav-header-text text-transparent transition-all hover:-mt-2">
            Websites,
        </h1>
        <h1 class="text-8xl ml-12 cursor-pointer nav-header-text text-transparent transition-all hover:-mt-2">
            Apps,
        </h1>
        <h1 class="text-8xl ml-12 cursor-pointer nav-header-text text-transparent transition-all hover:-mt-2">
            Bots
        </h1>
    </section>
</template>

<script>
export default {
    name: 'Developer',
    props: ['name', 'description', 'tag', 'profilePhoto']
}
</script>

<style scoped>
.nav-header-text {
    -webkit-text-stroke: 2px #7c3aed;
}

.nav-header-text:hover {
    -webkit-text-stroke: 2px white;
    color: white;
}
</style>