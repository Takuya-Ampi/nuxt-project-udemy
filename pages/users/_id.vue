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
  },
  // バリデーションに関しては,Nuxt公式に書いてある
  // 参考 https://ja.nuxtjs.org/api/pages-validate/
  // /^\d+$/は正規表現
  // 数値でなければならない
  validate({ params }){
    return /^\d+$/.test(params.id)
  }
};
</script>

<style>
</style>
