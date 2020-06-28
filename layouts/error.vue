<template>
  <section class="container">
    <!-- v-ifはなくても良い -->
    <p v-if="error.statusCode === 404">エラー 404</p>
  </section>
</template>

<script>
export default {
  // 下記記述によりステータスコードを受け取ることができるようになる
  props: ['error']
};
</script>

<style>
</style>
