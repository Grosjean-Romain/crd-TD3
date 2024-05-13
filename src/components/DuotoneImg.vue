<script setup lang="ts">
defineProps<{
  imgAlt: string
  imgPath: string
  classPicture?: string
  classImg?: string
}>()
</script>

<template>
  <picture
    class="relative flex overflow-hidden bg-pink before:absolute before:inset-0 before:z-[1] before:bg-indigo before:mix-blend-lighten before:transition-all before:duration-300 before:ease-in-out"
    :class="classPicture">
    <img class="flex-[1_0_100%] object-cover mix-blend-multiply grayscale" :src="imgPath" :alt="imgAlt" :src="imgPath"
      :alt="imgAlt" />
  </picture>
</template>