<script setup>
import { ref } from 'vue'

const nome = ref('')
const email = ref('')
const senha = ref('')
const senha1 = ref('')
</script>

<template>

  <div>
    <p>Nome: </p>
    <input type="text" v-model="nome" placeholder="Digite seu nome" />
    <p>Email: </p>
    <input type="email" v-model="email" placeholder="Digite seu email" />
    <p>Senha: </p>
    <input type="password" v-model="senha" placeholder="Digite sua senha" />
    <p>Confirmar senha: </p>
    <input type="password" v-model="senha1" placeholder="Digite sua senha" />
    <div v-if="senha = senha1">
      ta certa a senha
    </div>
    <div v-else>
      a senha ta errada
    </div>
  </div>

</template>

<style scoped>

</style>
