<template>
  <div>
    <Label class="block mb-2 text-sm font-medium text-gray-900" :label="id" :text="text" />
    <Input class="w-full bg-gray-50 border border-gray-300 text-gray-900 sm:text-sm rounded-lg focus:ring-primary-600 focus:border-primary-600 block p-2.5" :type="type" :name="name" :id="id" :placeholder="placeholder" :value="value" />
  </div>
</template>

<script setup lang="ts">
import Label from '@/components/atoms/Label.vue'
import Input from '@/components/atoms/Input.vue'

const props = withDefaults(defineProps<{
  text: string,
  type?: string,
  name?: string,
  id?: string,
  placeholder?: string,
  value?: string | number
}>(), {
})
</script>
