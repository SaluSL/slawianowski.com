<script setup lang="ts">
const props = defineProps<{
  to: string;
  label: string;
}>();
</script>

<template>
  <NuxtLink
    :to="props.to"
    class="py-1 px-2 rounded-md text-gray-600 hover:bg-gray-200 hover:text-gray-900 font-semibold"
    active-class="bg-gray-600 text-white"
    >{{ label }}<slot></slot
  ></NuxtLink>
</template>
