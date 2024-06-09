<template>
  <div
      v-editable="blok"
      class="w-full bg-gray-100"
  >
    <div class="flex max-w-screen-2xl mx-auto">
      <div class="text-lg sm:text-2xl font-bold text-start place-self-center m-5 mr-8">
        {{ blok.title }}
      </div>
      <div class="container flex gap-3 place-items-center">
        <StoryblokComponent
            v-for="blok in blok.nav_links"
            :key="blok._uid"
            :blok="blok"
        />
      </div>
    </div>
  </div>
</template>

<script setup>
defineProps({blok: Object})
</script>
