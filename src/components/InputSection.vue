<template>
  <section class="py-5 shadow-black">
    <div class="container">
      <form class="form items-center" @submit.prevent="submit">
        <div class="field">
          <label for="name">Name</label>
          <input id="name" type="text" v-model="form.name" />
        </div>
        <div class="field">
          <label for="content">Content</label>
          <input id="content" type="text" v-model="form.content" />
        </div>
        <input type="submit" class="hidden" />
      </form>
    </div>
  </section>
</template>

<script setup lang="ts">
  import { reactive } from 'vue'

  let form = reactive({ name: '', content: '' })

  const submit = () => {
    console.log('submit', { form })
  }
</script>

<style scoped>
  .form {
    @apply space-y-2 md:flex md:space-x-4 md:space-y-0;
  }

  .field {
    @apply flex flex-col space-y-3;

    label {
      @apply text-gray-500 text-sm underline decoration-fontech decoration-4;
    }

    input {
      @apply border border-gray-300 rounded-lg p-2;
    }

    &:nth-child(2) {
      @apply flex-1;
    }
  }
</style>
