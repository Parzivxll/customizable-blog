<template>
  <main class="container mx-auto py-16 w-full">
    <Developer :tag="developer.tag" :description="developer.description" :name="developer.name"
      :profilePhoto="developer.profilePhoto" />
    <Categories class="mt-8" />
    <Projects class="mt-12" />
    <Techstack class="mt-12" />
  </main>
</template>

<script>
import Developer from "../components/home/Developer.vue";
import Projects from "../components/home/Projects.vue";
import Techstack from "../components/home/Techstack.vue";
import Categories from "../components/home/Categories.vue";

export default {
  name: "Home",
  components: {
    Developer,
    Projects,
    Techstack,
    Categories
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
