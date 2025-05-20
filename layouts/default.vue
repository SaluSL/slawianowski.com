<script lang="ts" setup>
import Link from "~/components/ui/Link.vue";
</script>

<template>
  <div class="flex flex-col h-screen">
    <header class="bg-gray-100 text-whit p-4">
      <nav>
        <ul class="flex space-x-2 sm:space-x-8 justify-center">
          <li>
            <Link to="/" label="Home" />
          </li>
          <li>
            <Link to="/projects" label="Projects" />
          </li>
          <li>
            <Link to="/blog" label="Blog" />
          </li>
          <li>
            <Link to="/contact" label="Contact" />
          </li>
        </ul>
      </nav>
    </header>
    <main class="flex-1 p-4 container mx-auto">
      <slot />
    </main>
    <footer class="bg-gray-100 text-sm text-gray-600 p-4">
      <p>&copy; {{ new Date().getFullYear() }} slawianowski.com</p>
    </footer>
  </div>
</template>

<style>
body {
  background-color: #f9fafb;
}
</style>
