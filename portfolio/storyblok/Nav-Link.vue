<template>
  <NuxtLink
      v-editable="blok"
      :to="blok.link.url"
  >
    <div
        v-editable="blok"
        class="text-center text-sm sm:text-xl transition duration-300 ease-in-out hover:bg-gray-200 hover:rounded-lg p-2"
    >
      {{ blok.text }}
    </div>
  </NuxtLink>
</template>

<script setup>
defineProps({blok: Object})
</script>
