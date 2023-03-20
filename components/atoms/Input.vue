<template>
  <input :type="type" :name="name" :id="id" :placeholder="placeholder" :value="value">
</template>

<script setup lang="ts">

interface Props {
  type?: string,
  name?: string,
  id?: string,
  placeholder?: string,
  value?: string | number
}

const props = withDefaults(defineProps<Props>(), {
  type: 'text',
  name: '',
  id: '',
  placeholder: '',
  value: ''
})
</script>
