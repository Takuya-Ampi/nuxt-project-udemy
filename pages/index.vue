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

      <!-- vuex -->
      <!-- vuex stateの参照 -->
      <!-- <p>{{ $store.state.message }}</p> -->
      <!-- vuex stateの更新(ミューテーション) -->
      <!-- <button @click="$store.commit('updateMessage')">Update</button> -->

      <!-- vuex stateの更新(ミューテーション,値渡し[payload]) -->
      <!-- <button @click="$store.commit('updateMessage', 'Commit with payload')">Update</button> -->


      <!-- vuex stateの更新(アクション) -->
      <!-- <button @click="$store.dispatch('updateMessageAction')">Dispatch</button> -->
      <!-- <button @click="$store.dispatch('updateMessageAction', 'Dispatch with payload')">Dispatch</button> -->

      <!-- カウンターアプリの作成 -->
      <Counter></Counter>
      <Counter></Counter>
      <Counter></Counter>

    </div>
  </section>
</template>

<script>
// const axios = require("axios");
// let url = "https://jsonplaceholder.typicode.com/usersxxx";

// カウンターアプリの作成
import Counter from '~/components/Counter.vue'

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

  // カウンターアプリの作成
  components: {
    Counter
  }
};
</script>

<style>
p {
  font-family: "A-OTF Ryumin Pro";
}
</style>
