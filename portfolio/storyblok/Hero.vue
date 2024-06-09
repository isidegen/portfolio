<template>
  <div id="hero"
      v-editable="blok"
      class="h-[60vh] py-32 px-4 h-5/6 place-content-center"
  >
    <div
        class="pb-5 text-6xl font-bold text-center max-w-3xl mx-auto"
    >
      {{ blok.title }}
    </div>
    <div
        class="text-4xl text-center text-neutral-700 max-w-3xl mx-auto"
    >
      {{ blok.subtitle }}
    </div>
  </div>
</template>

<script setup>
defineProps({blok: Object})
</script>
