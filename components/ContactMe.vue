<script setup lang="ts"></script>
<template>
  <h2 class="font-semibold text-xl text-center">Find me on:</h2>
  <ul class="flex gap-8 mt-4 justify-center w-full">
    <li>
      <NuxtLink to="https://github.com/SaluSL">
        <Icon name="uil:github" class="text-2xl" />
        <span class="sr-only">Github</span>
      </NuxtLink>
    </li>
    <li>
      <NuxtLink to="https://linkedin.com/in/slawianowski">
        <Icon name="uil:linkedin" class="text-2xl" />
        <span class="sr-only">Linkedin</span>
      </NuxtLink>
    </li>
    <li>
      <NuxtLink to="mailto:szymon@slawianowski.com">
        <Icon name="lucide:mail" class="text-2xl" />
        <span class="sr-only">Email</span>
      </NuxtLink>
    </li>
  </ul>
</template>
