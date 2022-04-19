<template>
    <section id="index" class="flex items-center justify-between">
        <div class="w-[512px]">
            <h3 class="text-5xl mb-4 font-bold">
                {{ name }}
            </h3>
            <p class="text-lg">
                {{ description }}
            </p>
            <div class="flex flex-wrap items-center mt-8 gap-2">
                <IconButton class="px-4 py-2 rounded-xl bg-secondary hover:brightness-125 transition"
                    v-for="(link, i) in links" :key="i" :name="link.name" :icon="link.icon"
                    iconClass="w-6 h-6 fill-white mr-2" @click="navigate(link.url)" />
            </div>
        </div>
        <div class="relative">
            <img class="rounded-3xl h-full w-full cliped-image w-72 h-72" :src="profilePhoto" alt="Profile Photo" />
            <div
                class="absolute bottom-0 left-1/2 -translate-x-1/2 bg-tertiary font-medium text-lg px-8 w-max py-2 rounded-xl cursor-pointer transition hover:brightness-125">
                Full-stack dev.</div>
        </div>
    </section>
</template>

<script>
import { defineComponent } from "vue";
import IconButton from "@/components/common/IconButton.vue";
import GithubSvg from "@/assets/svg/github.svg"
import DiscordSvg from "@/assets/svg/discord.svg"
import MailSvg from "@/assets/svg/mail.svg"
import LinkedInSvg from "@/assets/svg/linkedin.svg"

export default defineComponent({
    name: 'Developer',
    props: ['name', 'description', 'tag', 'profilePhoto'],

    components: {
        IconButton
    },

    data() {
        return {
            links: [
                {
                    name: "Github",
                    icon: GithubSvg,
                    url: "https://github.com/serendiasquad/"
                },
                {
                    name: "Discord",
                    icon: DiscordSvg,
                    url: "https://discord.gg/serendia"
                },
                {
                    name: "Mail",
                    icon: MailSvg,
                    url: "team@serendiasquad.org"
                },
                {
                    name: "LinkedIn",
                    icon: LinkedInSvg,
                    url: "https://github.com/JeParzival"
                }
            ]
        }
    },

    methods: {
        navigate(url) {
            window.open(url, "_blank");
        }
    }
})
</script>

<style scoped>
.cliped-image {
    clip-path: polygon(30% 0%, 70% 0%, 100% 30%, 100% 70%, 70% 100%, 30% 100%, 0% 70%, 0% 30%);
}
</style>
