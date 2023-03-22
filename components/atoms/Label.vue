<template>
  <label :for="label">
    {{ text }}
  </label>
</template>
<script setup lang="ts">

interface Props {
  label?: string,
  text: string
}

const props = withDefaults(defineProps<Props>(), {
  label: '',
  text: ''
})
</script>
