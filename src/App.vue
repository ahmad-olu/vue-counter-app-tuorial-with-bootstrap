<script setup>
import { ref } from "vue";
import "bootstrap/dist/css/bootstrap.css";
import "bootstrap/dist/js/bootstrap.js";
const count = ref(0);
</script>

<template>
  <main >
    <div >
      <h4>The current count is...</h4>
        <h1 >{{count}}</h1>
        <button @click="count--" class="btn btn-outline-dark btn-outline-dark button button1">-</button>
        <button @click="count++" class="btn btn-outline-dark btn-outline-dark button button1">+</button>
    </div>
  </main>
</template>

<style scoped>
main {
    width: 100vw;
    height: 100vh;
    background-color: palegreen;
    display: flex;
    align-items: center;
    justify-content: center;
}

div{
    text-align: center;
    text-decoration: solid;
    text-shadow: 30%;
    color: black;
    
}

.button1 {padding: 10px 24px;margin-right: 20px;margin-left: 20px; text-decoration: solid;
}
</style>
