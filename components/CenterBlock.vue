<script setup>
const props = defineProps({
    isRow: {
        type: Boolean,
        default: false,
    }
})
</script>

<template>
    <div class="h-full flex justify-center items-center pb-8" :class="{'flex-col': !props.isRow}">
        <slot />
    </div>
</template>