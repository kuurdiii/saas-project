<template>
    <input class="border-0 p-1 px-2 font-semibold autofill:bg-blue-300 autofill:rounded-sm text-white bg-transparent placeholder-gray-500 focus:ring-0 sm:text-sm md:text-xl" :value="modelValue" @input="$emit('update:modelValue', $event.target.value)" ref="input">
</template>

<script>
    import { defineComponent } from 'vue'

    export default defineComponent({
        props: ['modelValue'],

        emits: ['update:modelValue'],

        methods: {
            focus() {
                this.$refs.input.focus()
            }
        }
    })
</script>
