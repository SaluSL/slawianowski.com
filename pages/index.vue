<script setup lang="ts">
import ContactMe from "~/components/ContactMe.vue";
</script>

<template>
  <div
    class="w-full flex flex-col items-center justify-center h-full 2xl:gap-16"
  >
    <div class="">
      <NuxtImg
        src="animated.png"
        alt="Szymon Sławianowski"
        class="rounded-full w-32 2xl:w-64 h-32 2xl:h-64 mb-4"
      ></NuxtImg>
    </div>
    <div>
      <h1 class="text-center text-2xl font-medium">
        Hi, I'm Szymon Sławianowski
      </h1>
      <p class="text-center text-lg mt-4 max-w-prose">
        I'm a software engineer with a passion for building and scaling
        products. I have experience in various domains, including web
        development and cloud computing. I love to learn new technologies and
        apply them to solve real-world problems.
      </p>
    </div>

    <div class="mt-8 2xl:mt-12">
      <ContactMe />
    </div>
  </div>
</template>
