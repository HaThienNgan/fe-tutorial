<template>
  <NuxtLink :to="to" class="font-bold p-2 rounded-md text-slate-500 text-center hover:text-slate-900 hover:bg-slate-100 ">
    {{ text }}
  </NuxtLink>
</template>

<script>
export default {
  props: {
    text: {
      type: String,
      required: false,
      default: ""
    },
    to: {
      type: String,
      required: true
    }
  }
}
</script>
