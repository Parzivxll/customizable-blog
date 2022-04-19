<template>
    <div class="bg-secondary hover:brightness-125 transition cursor-pointer rounded-lg px-4 py-2">
        <slot></slot>
    </div>
</template>

<script>
export default {
    name: 'Card',
    props: ['title', 'description', "image",]
}
</script>