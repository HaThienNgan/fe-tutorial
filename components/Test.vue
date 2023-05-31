<template>
  <div>
    {{ name }}
    <img src="/images/logo.png" alt="Logo" />
  </div>
</template>

<script>
export default {
  props: {
    name: {
      type: String,
      required: false,
      default: ""
    }
  }
}
</script>
