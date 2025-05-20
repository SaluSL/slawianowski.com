<script setup lang="ts">
const copyEmailToClipboard = (text: string) => {
  navigator.clipboard.writeText(text);
  mailCopiedToClipboard.value = true;
  setTimeout(() => {
    mailCopiedToClipboard.value = false;
  }, 3000);
};
const mailCopiedToClipboard = ref(false);
</script>

<template>
  <div class="flex flex-col items-center justify-center h-full text-center">
    <div class="flex items-center gap-2 mb-8 2xl:mb-16">
      <Icon name="lucide:mail" class="text-3xl" />

      <div class="flex gap-2 items-center">
        <NuxtLink to="mailto:szymon@slawianowski.com">
          szymon@slawianowski.com</NuxtLink
        >
        <div v-if="mailCopiedToClipboard" class="text-green-500">
          <span class="sr-only">Email copied to clipboard!</span
          ><Icon name="lucide:copy-check" class="text-xl" />
        </div>
        <button @click="copyEmailToClipboard('szymon@slawianowski.com')" v-else>
          <span class="sr-only">Copy email</span>

          <Icon name="lucide:copy" class="text-xl" />
        </button>
      </div>
    </div>
    <ContactMe />
  </div>
</template>
