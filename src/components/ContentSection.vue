<template>
  <main class="mb-auto flex bg-gray-100 overflow-y-auto">
    <div class="container pt-8 space-y-4">
      <div
        class="w-52 p-5 bg-white rounded break-all md:w-96"
        v-for="{ content, id } in contents"
        :key="id"
      >
        {{ content }}
      </div>
    </div>
  </main>
</template>

<script setup lang="ts">
  import { ref } from 'vue'

  const contents = ref([
    { id: '1', content: 'PHP也有Day #63' },
    { id: '2', content: '前後端分離實戰應用，帶你半小時內實作「留言板」' },
    { id: '3', content: 'Decoupled Architecture' },
    {
      id: '4',
      content:
        '前後端分離的開發方法在軟體圈已經耳聞好一陣子，但實際應用在專案上的介紹，不論是在網路上或是任何的文獻上面幾乎是屈指可數。Decoupled Architecture 前後端分離開發方法，現今已經廣泛被應用在每一個我們所開發的專案上，無論是在工程師之間的溝通、開發的效率、開發的時程和程式碼的易讀性都比以往的開發大躍進許多。這次的 PHP 也有 Day 聚會上將會介紹如何用 Laravel + GraphQL + Nuxt 的綜合體結合，半小時內即可獲得「留言板」。同場加映！更深入的探討 Lighthouse 與 Apollo 等等的應用。',
    },
    { id: '5', content: 'Sasaya~~~~~~~~~~~Sasaya~~~~~~~~~~~' },
    {
      id: '6',
      content:
        'Sasaya，Fontech 技術長，目前致力於推廣 Vim + Tmux 的黑畫面開發模式。對極速且高品質的開發相當有興趣。為了加速開發而做了許多小工具，如 Babel 插件或Vim 插件。業餘時間的興趣是玩打擊樂。',
    },
    { id: '7', content: 'Fontech~~~~~~~~~~~Fontech~~~~~~~~~~~' },

    { id: '8', content: '大瀚環球商務中心/台北市信義區忠孝東路四段560號8樓' },
    { id: '9', content: '1月18日 (二) 19:00' },
  ])
</script>

<style scoped>
  main > div:last-child::after {
    content: '';

    @apply h-8 block;
  }
</style>
