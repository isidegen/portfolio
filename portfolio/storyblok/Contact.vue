<template>
  <div
      v-editable="blok"
      class="py-8 px-8 sm:flex max-w-5xl justify-center items-center mx-auto">
    <div class="p-10">
      <img
          v-if="blok.image?.filename"
          :src="blok.image.filename + '/m/1600x0'"
          :alt="blok.image.alt"
          class="w-[250px] object-cover rounded-2xl shadow-xl"
      />
    </div>
      <div class="space-y-2">
        <div class="text-xl font-bold">
          {{ blok.name }}
        </div>
        <div class="text-xl">
          {{ blok.email }}
        </div>
        <p>
          {{ blok.more }}
        </p>
      </div>

  </div>
</template>

<script setup>
defineProps({blok: Object})
</script>
