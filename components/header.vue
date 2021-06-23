<template>
  <div class="bg text-gray-50">
    <div class="grid grid-cols-2 text-lg tracking-wide">
      <nuxt-link :to="{ path: '/' }">Artur Teixeira</nuxt-link>
      <span class="text-right links">
        <nuxt-link :to="{ path: '/', hash: '#how' }">how I work</nuxt-link>
        <nuxt-link :to="{ path: '/', hash: '#about' }">about</nuxt-link>
        <nuxt-link :to="{ path: '/', hash: '#contact' }">contact</nuxt-link>
      </span>
    </div>
    <div class="h-full flex justify-center">
      <div class="text-3xl font-light cover-txt">
        <div>
          Discuss, Organize and Develop applications that bring value. <br />
          <nuxt-link :to="{ path: '/', hash: '#contact' }"
            >Contact me</nuxt-link
          >
          for a <span class="font-normal">free</span> 30-min consultation.
        </div>
      </div>
    </div>
  </div>
</template>
<script lang="ts">
export default {
  name: 'Header',
}
</script>
<style>
.bg {
  background-image: url('~assets/hero-image.jpg');
  background-size: cover;
  background-position: center;

  height: 80vh;
  padding: 16px;
}

.links > a {
  margin-right: 10px;
  text-decoration: underline;

  @media (max-width: 520px) {
    display: flex;
    justify-content: flex-end;
  }
}

.cover-txt {
  width: 900px;
  align-self: center;
  margin: 16px;
}
</style>