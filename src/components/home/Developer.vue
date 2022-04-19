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
                <IconButton class="px-4 py-2 rounded-3xl bg-secondary hover:brightness-125 transition"
                    v-for="(link, i) in links" :key="i" :name="link.name" :icon="link.icon"
                    iconClass="w-6 h-6 fill-white mr-2" @click="" />
            </div>
        </div>
        <div class="relative w-96 h-96 p-3 bg-secondary flex items-center justify-center rounded-3xl">
            <img class="rounded-3xl h-full w-full" :src="profilePhoto" alt="Profile Photo" />
            <div
                class="absolute bottom-0 translate-y-1/2 bg-secondary w-48 rounded-3xl h-16 flex items-center justify-center">
                <span class="text-xl font-medium">{{ tag }}</span>
            </div>
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
                    URL: "https://github.com/serendiasquad/"
                },
                {
                    name: "Discord",
                    icon: DiscordSvg,
                },
                {
                    name: "Mail",
                    icon: MailSvg
                },
                {
                    name: "LinkedIn",
                    icon: LinkedInSvg
                }
            ]
        }
    }
})
</script>
