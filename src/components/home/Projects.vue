<template>
    <section>
        <div>
            <span class="text-2xl font-medium">featured </span>
            <span class="text-2xl font-bold text-white-stroke text-transparent">projects</span>
        </div>

        <div class="mt-4 grid grid-cols-4 gap-2 w-full">
            <Card :title="project.name" :description="project.description" v-for="project in projects">
                <a :href="project.url">
                    <h1 class="text-xl mb-2 font-medium">{{ project.name }}</h1>
                    <p class="text-base">{{ project.description }}</p>
                </a>
            </Card>
        </div>
    </section>
</template>

<script>
import Card from "../Common/Card.vue";

export default {
    name: "Projects",
    components: {
        Card,
    },

    data() {
        return {
            projects: [
                {
                    name: 'React.js',
                    description: 'for me, thats an a js framework not library. i believe that! adssadasdsad',
                    url: "https://github.com/facebook/react/"
                },
                {
                    name: 'React.js',
                    description: 'for me, thats an a js framework not library. i believe that! adssadasdsad',
                    url: "https://github.com/facebook/react/"
                }, {
                    name: 'React.js',
                    description: 'for me, thats an a js framework not library. i believe that! adssadasdsad',
                    url: "https://github.com/facebook/react/"
                }, {
                    name: 'React.js',
                    description: 'for me, thats an a js framework not library. i believe that! adssadasdsad',
                    url: "https://github.com/facebook/react/"
                }, {
                    name: 'React.js',
                    description: 'for me, thats an a js framework not library. i believe that! adssadasdsad',
                    url: "https://github.com/facebook/react/"
                }, {
                    name: 'React.js',
                    description: 'for me, thats an a js framework not library. i believe that! adssadasdsad',
                    url: "https://github.com/facebook/react/"
                }, {
                    name: 'React.js',
                    description: 'for me, thats an a js framework not library. i believe that! adssadasdsad',
                    url: "https://github.com/facebook/react/"
                }, {
                    name: 'React.js',
                    description: 'for me, thats an a js framework not library. i believe that! adssadasdsad',
                    url: "https://github.com/facebook/react/"
                }, {
                    name: 'React.js',
                    description: 'for me, thats an a js framework not library. i believe that! adssadasdsad',
                    url: "https://github.com/facebook/react/"
                }, {
                    name: 'React.js',
                    description: 'for me, thats an a js framework not library. i believe that! adssadasdsad',
                    url: "https://github.com/facebook/react/"
                },
            ],
        }
    }
};
</script>
