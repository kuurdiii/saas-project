<template>
    <label class="block text-xs mx-2 mt-1 font-normal focus-within:text-blue-700 text-gray-200">
        <span v-if="value">{{ value }}</span>
        <span v-else><slot></slot></span>
    </label>
</template>

<script>
    import { defineComponent } from 'vue'

    export default defineComponent({
        props: ['value']
    })
</script>
