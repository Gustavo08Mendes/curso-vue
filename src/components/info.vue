<template>
  <div>
    <h1>Esta é a descrição da Pessoa: {{ nome }}</h1>
    <p v-if="estra_trabalhando">Estou trabalhando no momento</p>
    <p v-else>Estou em busaca de novas oportunidades</p>
    <button @click="showEmail">{{ valorBotao }}</button>
    <p v-show="mostrarEmail">Meu email: {{ email }}</p>
    <p>Utilizo as seguintes tecnologias para back-end:</p>
    <ul>
      <li v-for="(technology, index) in backend_tecnologes" v-bind:key="index">
        {{ technology }}
      </li>
    </ul>
    <p>Utilizo as seguintes tecnologias para front-end:</p>
    <ul>
      <li v-for="(technology, index) in frontend_tecnologes" v-bind:key="index">{{ technology.language }}</li>
    </ul>
  </div>
</template>
<script>
export default {
  name: "Info",
  data() {
    return {
      estra_trabalhando: true,
      mostrarEmail: false,
      email: "bS3pG@example.com",
      valorBotao: "Mostrar email",
      backend_tecnologes: ["JavaScript", "PHP", "Python"],
      frontend_tecnologes: [
        {id: 1, language: "HTML"},
        {id: 2, language: "CSS"},
        {id: 3, language: "VueJS"},
      ],
    };
  },
  methods: {
    showEmail() {
      this.mostrarEmail = !this.mostrarEmail;
    },
  },
};
</script>
