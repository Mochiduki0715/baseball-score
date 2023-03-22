<template>
<div class="flex items-center">
  <div class="flex items-center">
    <Input class="w-4 h-4 border border-gray-300 rounded bg-gray-50 focus:ring-3 focus:ring-primary-300" type="checkbox" :id="id" />
  </div>
  <div class="ml-3 text-sm">
    <Label class="text-gray-500" :label="id" :text="text" />
  </div>
</div>
</template>
<script setup lang="ts">
import Input from '@/components/atoms/Input.vue'
import Label from '@/components/atoms/Label.vue'

const props = withDefaults(defineProps<{
  id: string,
  text: string
}>(), {

})
</script>
