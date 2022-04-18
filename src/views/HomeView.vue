<template>
  <main class="container mx-auto py-12 w-full">
    <Developer :tag="developer.tag" :description="developer.description" :name="developer.name"
      :profilePhoto="developer.profilePhoto" />
    <Projects />
    <Techstack />
  </main>
</template>

<script>
import Developer from "../components/home/Developer.vue";
import Projects from "../components/home/Projects.vue";
import Techstack from "../components/home/Techstack.vue";

export default {
  name: "Home",
  components: {
    Developer,
    Projects,
    Techstack,
  },

  computed: {
    developer() {
      return {
        name: "Mert Yılmaz",
        description:
          "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Possimus quod delectus quibusdam accusamus hic, ea veniam, facilis eveniet nisi corporis minus minima eos ipsam est doloribus dolore. Eius, placeat consectetur!",
        tag: "Full-stack dev.",
        profilePhoto:
          "https://cdn.discordapp.com/avatars/956157077083013150/591fe2354288c8976c6a7619f519f0eb.png",
      };
    },
  },
};
</script>
