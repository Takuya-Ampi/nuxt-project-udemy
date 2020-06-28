<template>
  <section class="container">
    <h2>{{ title }}</h2>
    counter: {{ $store.state.counter.counter }}
    <button @click="$store.commit('counter/countUp')">+1</button>

  </section>
</template>

<script>
export default {
  data(){
    return {
      title: 'Counter APP'
    }
  }

};
</script>

<style>
</style>
