<template>
    <section>
        <span class="text-2xl font-medium">tech</span><span
            class="text-2xl text-white-stroke font-bold text-transparent">stack</span>

        <div class="mt-4 flex gap-4">
            <Card class="w-24 h-24 flex items-center justify-center" v-for="techstack in techstacks"
                :title="techstack.name" :image="techstack.image">
                <img :src="techstack.image" />
            </Card>
        </div>
    </section>
</template>

<script>
import Card from "../Common/Card.vue";

export default {
    name: "Techstack",
    components: {
        Card,
    },

    data() {
        return {
            techstacks: [
                {
                    name: "HTML5",
                    image: "https://logos-download.com/wp-content/uploads/2017/07/HTML5_badge-700x700.png",
                },
                {
                    name: "JS",
                    image: "https://logos-download.com/wp-content/uploads/2019/01/JavaScript_Logo-700x700.png",
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
            ],
        }
    }
};
</script>
