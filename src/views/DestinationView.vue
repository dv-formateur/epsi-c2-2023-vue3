<script>
export default {
  computed: {
    destinationSentence() {
      return `Notre destination sera ${this.$route.params.pays}`
    }
  }
}
</script>

<template>
  <div>
    <h1>Ma page destination : {{ $route.params.pays }}</h1>
    <div>{{ destinationSentence }}</div>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
