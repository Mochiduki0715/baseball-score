<template>
  <button type="button" class="w-full focus:ring-4 focus:outline-none focus:ring-primary-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center">
    {{ text }}
  </button>
</template>

<script setup lang="ts">

interface Props {
  text: string
}

const props = withDefaults(defineProps<Props>(), {
  text: ''
})
</script>