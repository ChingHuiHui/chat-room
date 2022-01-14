<template>
  <main class="flex">
    <div class="container border-x flex flex-col">
      <section class="flex-1 bg-gray-700">chat contents</section>

      <section class="bg-gray-500 w-full p-5">
        <form action="" class="flex space-x-4">
          <input type="text" />
          <input type="text" />
        </form>
      </section>
    </div>
  </main>
</template>

<script setup></script>

<style scoped>
  main {
    @apply w-full h-full;
  }

  input {
    @apply border px-2 py-4;
  }
</style>
