<!-- COUNTER APP SCRIPT -->
<script setup>
import { ref } from "vue";
const count = ref(0);
</script>

<!-- COUNTER APP TEMPLATE -->
<template>
  <div id="app">
    <h4>The current count is...</h4>
    <h1>{{  count }}</h1>
    <span>
        <button @click="count--">-</button>
        <button @click="count++">+</button>
    </span>
</div>
</template>

<!-- COUNTER APP STYLE -->
<style scoped>
#app{
    text-align: center;
}
#app button{
  font-size:30px;
  background-color:hsl(26, 71%, 48%);
  padding: 15px 40px;
  border-radius: 10px;
  border:1px solid hsl(26, 71%, 48%);
  margin-right:10px;
}

#app button:focus{
    transform: scale(0.9);
    transition:all '42s;'
}
</style>

