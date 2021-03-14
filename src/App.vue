<template>
  <v-app>
    <v-main>
      <div class="center"> 
        <v-btn icon="mdi-minus" @click="state.counter--"></v-btn>
        <h1 class="ma-3">{{state.counter}}</h1>
        <v-btn icon="mdi-plus" @click="state.counter++"></v-btn>
      </div>
    </v-main>
  </v-app>
</template>

<script setup>
import { reactive } from "vue"

const state = reactive({ counter: 0})
</script>

<style>
.center {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}
</style>
