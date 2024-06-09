<template>
  <div
      v-editable="blok"
      :id="blok.sectionname"
      class="py-20 px-4"
  >
    <div
        v-editable="blok"
        class=" text-3xl font-bold text-center max-w-3xl mx-auto"
    >
      {{ blok.title }}
    </div>
    <div
        v-editable="blok"
        class="text-2xl text-center text-neutral-700 max-w-3xl mx-auto"
    >
      {{ blok.subtitle }}
    </div>
    <StoryblokComponent
        v-for="blok in blok.blocks"
        :key="blok._uid"
        :blok="blok"
    />
  </div>
</template>

<script setup>
defineProps({blok: Object})
</script>
