<template>
  <div class="grid grid-cols-2 p-4 border-t-2 border-blue-900">
    <div>
      Artur Teixeira<br />
      info@artur-teixeira.tech<br />
      <span
        class="underline text-blue-900 font-bold cursor-pointer"
        @click="scrollToTop"
      >
        Freelance Software Engineer</span
      >
    </div>
    <div class="text-right">
      i post regularly on:
      <a href="https://www.linkedin.com/in/arturjnt/" target="_blank">
        LinkedIn
      </a>
      <br />
      also, follow me on:
      <a href="https://twitter.com/arturjnt" target="_blank"> Twitter </a>
      <br />
      and check my open source work on:
      <a href="https://github.com/arturjnt/" target="_blank">
        GitHub
      </a>
    </div>
  </div>
</template>
<script lang="ts">
export default {
  name: 'Footer',
  methods: {
    scrollToTop(): void {
      window.scrollTo({ top: 0, behavior: 'smooth' })
    },
  },
}
</script>
<style scoped>
a {
  @apply underline text-blue-900 font-bold;
}
</style>