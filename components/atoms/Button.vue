<template>
  <button type="button" :disabled="isDisable" class="rounded-lg text-sm text-center">
    {{ text }}
  </button>
</template>

<script setup lang="ts">

interface Props {
  text: string,
  isDisable?: boolean
}

const props = withDefaults(defineProps<Props>(), {
  text: '',
  isDisable: false
})
</script>
