<template>
  <div
      v-editable="blok"
      class="py-8 px-8 sm:flex max-w-5xl justify-between items-center mx-auto">
    <template v-if="blok.image_right">
      <div class="space-y-2">
        <div class="text-3xl font-bold">
          {{ blok.title }}
        </div>
        <div class="text-xl">
          {{ blok.subtitle }}
        </div>
        <p>
          {{ blok.description }}
        </p>
      </div>
      <div class="p-10">
        <img
            v-if="blok.image?.filename"
            :src="blok.image.filename + '/m/1600x0'"
            :alt="blok.image.alt"
            class="w-96 h-96 object-cover rounded-2xl shadow-xl"
        />
      </div>
    </template>
    <template v-else>
      <div class="p-10">
        <img
            v-if="blok.image?.filename"
            :src="blok.image.filename + '/m/1600x0'"
            :alt="blok.image.alt"
            class="w-96 h-96 object-cover rounded-2xl shadow-xl"
        />
      </div>
      <div class="space-y-2">
        <div class="text-3xl font-bold">
          {{ blok.title }}
        </div>
        <div class="text-xl">
          {{ blok.subtitle }}
        </div>
        <p>
          {{ blok.description }}
        </p>
      </div>
    </template>
  </div>
</template>

<script setup>
defineProps({blok: Object})
</script>
