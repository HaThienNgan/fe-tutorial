<template>
  <div>
    <button @click="showCount = !showCount">Toggle Count</button>
    <div v-if="showCount">
      {{ count }}

    </div>
    <div v-else>
      Ga
    </div>

    <button @click="multiplicationBy10()">x10</button>

    <p v-if="$fetchState.pending">Loading....</p>
    <ul v-else>
      <li v-for="category in categories" :key="category.id">
        <LayoutsNavLink :text="category.name" :to="category.slug" />
      </li>
    </ul>
  </div>
</template>

<script>

export default {
  props: {
    test: {
      type: Number,
      required: false,
      default: 0
    }
  },
  data() {
    return {
      categories: [],
      mountains: [],
      count: 1,
      showCount: true
    }
  },
  computed: {
    doubleCount() {
      return this.count * 2
    }
  },
  methods: {
    multiplicationBy10() {
      this.count *= 10
      test *= 10
    }
  },
  async fetch() {
    try {
      const res = await this.$axios.get('https://api.apix.vn/marketplace/categories')
      this.categories = res.data.data
    } catch (e) {
      console.log(e)
    }
  }
}
</script>
