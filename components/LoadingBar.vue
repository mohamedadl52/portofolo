<template>
  <div v-if="loading" class="loading-page z-50">
    <p>Loading...</p>
  </div>
</template>

<script>
export default {
  data: () => ({
    loading: false,
  }),
  mounted() {
    this.$nextTick(() => {
      this.$nuxt.$loading.start()
      setTimeout(() => this.$nuxt.$loading.finish(), 2000)
    })
  },
  methods: {
    start() {
      this.loading = true
    },
    finish() {
      this.loading = false
    },
  },
}
</script>

<style scoped>
.loading-page {
  position: fixed;
  top: 0px;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(194, 130, 130, 1);
  text-align: center;
  padding-top: 200px;
  font-size: 30px;
  font-family: sans-serif;
}
</style>
