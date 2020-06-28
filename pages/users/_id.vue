<template>
  <section class="container">
    <p>{{ message }}</p>
    <p>id: {{ this.$route.params.id }}</p>
  </section>
</template>

<script>
export default {
  data() {
    return {
      message: "/users/_id.vue"
    };
  }
};
</script>

<style>
</style>
