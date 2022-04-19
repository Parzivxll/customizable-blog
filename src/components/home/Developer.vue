<template>
    <section id="index" class="flex justify-between">
        <div class="w-[512px]">
            <h3 class="text-5xl mb-4 font-bold">
                {{ name }}
            </h3>
            <p class="text-lg">
                {{ description }}
            </p>
            <div class="flex flex-wrap items-center mt-8 gap-2">
                <IconButton class="px-4 py-2 rounded-3xl bg-c2 hover:brightness-125 transition"
                    v-for="(link, i) in links" :key="i" :name="link.name" :icon="link.icon"
                    iconClass="w-6 h-6 fill-white mr-2" />
            </div>
        </div>
        <div class="relative w-64 h-64 p-3 bg-c2 flex items-center justify-center rounded-3xl">
            <img class="rounded-3xl h-full w-full" :src="profilePhoto" alt="Profile Photo" />
            <div class="absolute bottom-0 translate-y-1/2 bg-c2 w-48 rounded-3xl h-16 flex items-center justify-center">
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
