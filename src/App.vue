<script setup>
  import {ref,reactive} from 'vue';
  let nom=ref('Tom');
  function touche(e){
    nom.value=e.target.value;
  }
</script>

<template>
  <p>Le joueur {{nom}} a 500 points.</p>
  <p>Le joueur {{nom}} a fini le niveau 3.</p>
  <p>Le joueur {{nom}} est classé 4e.</p>
  Nom: <input @keyup="touche" />
</template>

<style scoped>
</style>