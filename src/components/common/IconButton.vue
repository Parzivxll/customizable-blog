<template>
    <button class="flex items-center" @click="this.$emit('click')">
        <component :is="icon" :class="iconClass" />
        <span>{{ name }}</span>
    </button>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
    name: "IconButton",
    props: ["name", "icon", "iconClass", "click"],

    mounted() {
        console.log(this.iconSize);
    }
});
</script>
