<template>
    <div class="bg-c2 hover:brightness-90 transition cursor-pointer rounded-lg px-4 py-2">
        <slot></slot>
    </div>
</template>

<script>
export default {
    name: 'Card',
    props: ['title', 'description', "image",]
}
</script>