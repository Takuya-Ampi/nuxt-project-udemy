<template>
  <section class="container">
    <!-- <p>{{ message }}</p>
    <router-link to="/price">Price Page</router-link>-->
    <div>
      <!-- {{ users[0].id }}, {{ users[0].name }} -->
      <!-- <ul>
        <li v-for="user in users" :key="user.id">{{ user.id }}, {{ user.name }},{{ user.company.name }};</li>
      </ul> -->
      <!-- <img src="~/assets/cat.jpg" alt=""> -->
      <p>{{ $store.state.message }};</p>
    </div>
  </section>
</template>

<script>
// const axios = require("axios");
// let url = "https://jsonplaceholder.typicode.com/usersxxx";

export default {
  // asyncData({ params, error }) {
  //   return axios.get(url)
  //     .then((res) => {
  //       // users:はマスタッシュ構文で表示するために設定
  //       return { users: res.data }
  //     })
  //     .catch((e => {
  //       // console.log(e.response.status);
  //       // error({users: e.response.status, message: e.message})
  //       error({users: e.response.status, message: 'error!!!!!'})
  //     }))
  // }
};
</script>

<style>
p {
  font-family: "A-OTF Ryumin Pro";
}
</style>
