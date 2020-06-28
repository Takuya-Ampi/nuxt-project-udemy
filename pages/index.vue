<template>
  <section class="container">
    <p>{{ message }}</p>
    <router-link to="/price">Price Page</router-link>
  </section>
</template>

<script>
export default {
  data() {
    return {
      message: "hello test"
    };
  }
};
</script>

<style>
p {
  font-family: 'A-OTF Ryumin Pro';
}
</style>
