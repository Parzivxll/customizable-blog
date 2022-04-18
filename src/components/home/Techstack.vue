<template>
    <div class="mt-8">
        <span class="text-2xl font-medium">tech</span>
        <span class="text-2xl text-white-stroke font-bold text-transparent">stack</span>
    </div>

    <div class="mt-4 grid grid-cols-12 gap-4">
        <Card v-for="techstack in techstacks" :title="techstack.name" :image="techstack.image">
            <img :src="techstack.image" />
        </Card>
    </div>
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
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
                },
                {
                    name: "CSS3",
                    image: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/2048px-CSS3_logo.svg.png"
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
