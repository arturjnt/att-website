<template>
  <div class="">
    <div class="tab__header">
      <a
        href="#"
        class="
          px-4 py-2
          bg-blue-900
          text-white
          border-b-2 border-white
          flex
          justify-between
        "
        @click.prevent="active = !active"
      >
        <div>{{ title }}</div>
        <span class="down-Arrow" v-show="!active">&#9660;</span>
        <span class="up-Arrow" v-show="active">&#9650;</span>
      </a>
    </div>
    <div class="tab__content p-2" v-show="active"><slot /></div>
  </div>
</template>
<script lang="ts">
export default {
  name: 'Accordion',
  props: ['title'],
  data() {
    return {
      active: false,
    }
  },
}
</script>