<template>
<div class="flex flex-col items-center justify-center px-6 py-8 mx-auto md:h-screen lg:py-0">
  <a href="#" class="flex items-center mb-6 text-2xl font-semibold">
    Baseball Score
  </a>
  <div class="w-full rounded-lg dark:border md:mt-0 sm:max-w-md xl:p-0">
    <div class="p-6 space-y-4 md:space-y-6 sm:p-8">
      <h1 class="text-xl font-bold leading-tight tracking-tight text-gray-900 md:text-2xl">
        Login your account
      </h1>
      <form class="space-y-4 md:space-y-6">
        <InputLabel text="email" id="email" type="email" />
        <InputLabel text="password" id="password" type="password" />
        <div class="flex items-center justify-between">
          <CheckBox id="remember" text="Remember me" />
          <a href="#" class="text-sm font-medium text-primary-600 hover:underline dark:text-primary-500">Forgot password?</a>
        </div>
        <button type="button" class="w-full bg-primary-600 hover:bg-primary-700 focus:ring-4 focus:outline-none focus:ring-primary-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center">Login</button>
        <p class="text-sm font-light text-gray-500 dark:text-gray-400">
          <a href="#" class="font-medium text-primary-600 hover:underline dark:text-primary-500">Sign up</a>
        </p>
      </form>
    </div>
  </div>
</div>
</template>
<script setup lang="ts">
import InputLabel from '@/components/molecules/InputLabel.vue'
import CheckBox from '@/components/molecules/CheckBox.vue'
</script>
