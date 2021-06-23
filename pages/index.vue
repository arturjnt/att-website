<template>
  <div class="full-page">
    <Header />
    <div class="my-container">
      <How-I-Work class="mw" />
      <About-Me class="mw p-4 border-2" />
      <Contact class="mw p-4 border-2 w-full" />
    </div>
    <Footer />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>

<style>
.full-page {
  min-width: 320px;
}

.my-container {
  @apply p-8 bg-gray-50;
  display: flex;
  flex-direction: column;
}
.mw {
  @apply mb-8 bg-white border-blue-900;
  max-width: 900px;
  align-self: center;
}
</style>
