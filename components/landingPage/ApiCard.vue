<template>
  <div class="border cursor-pointer rounded-lg p-4 hover:bg-slate-100">
    <img :src="imgSrc" alt="image" />
    <div class="font-medium text-lg mb-2"> {{ title }}</div>
    <div>{{ content }}</div>
  </div>
</template>

<script>
export default {
  props: {
    imgSrc: {
      type: String,
      required: false,
      default: "/images/composables-light.svg"
    },
    title: {
      type: String,
      required: false,
      default: ""
    },
    content: {
      type: String,
      required: true
    }
  }
}
</script>
