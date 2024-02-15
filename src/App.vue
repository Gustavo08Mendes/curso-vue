<template>
  <div>
    <Header />
    <PrimeiroComponente />
    <LifeCycle />
    <Pessoa />
  </div>
</template>

<script>
import PrimeiroComponente from "./components/PrimeiroComponente.vue";
import LifeCycle from "./components/LifeCycle.vue";
import Pessoa from "./components/pessoa.vue";
import Header from "./components/header.vue";

export default {
  name: "App",
  components: {
    Header,
    PrimeiroComponente,
    LifeCycle,
    Pessoa,
  },
};
</script>

<style>
body {
  background-color: #333;
  color: #fff;
}
li {
  color: aqua;
}
</style>
