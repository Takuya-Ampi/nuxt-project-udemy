<template>
  <section class="container">
    <!-- <p>{{ message }}</p>
    <router-link to="/price">Price Page</router-link>-->
    <div>
      {{ users[0].id }}, {{ users[0].name }}
    </div>
  </section>
</template>

<script>
const axios = require("axios");
let url = "https://jsonplaceholder.typicode.com/users";

export default {
  asyncData({ params }) {
    return axios.get(url)
      .then((res) => {
        // users:はマスタッシュ構文で表示するために設定
        return { users: res.data }
      })
  }
};
</script>

<style>
p {
  font-family: "A-OTF Ryumin Pro";
}
</style>
