<template>
<header class="header">
  <h2>Фотостудия салют</h2>
</header>

<input class="input" type="text" v-model="number1" placeholder="Фамилия" maxlength="10">
<br>
<input class="input" type="text" v-model="number2" placeholder="Имя" maxlength="10">
<br>
<input class="input" type="text" v-model="number3" placeholder="Отчество" maxlength="10">
<br>
<input class="input" type="text" v-model="number4" placeholder="+7(000)000-00-00">
<br>
<input class="input" type="text" v-model="number5" placeholder="Кол-во дней" maxlength="2" />

<br>
<br>
<button class="btn"  @click="SendData"> Отправить </button>

<footer class="footer">
  @все права защищены 2025
</footer>
</template>

<script setup>
import { ref } from 'vue'

const number1 = ref("")
const number2 = ref("")
const number3 = ref("")
const number4 = ref("")
const number5 = ref("")

const SendData = true

</script>

<style scoped>
.header{
  margin-top: -300px;
  background-color: rgba(71, 71, 71, 0.703);
  width: 100vw;
  margin-left: -125px;
  height: 50px;
}

.footer{

  background-color: rgba(118, 118, 118, 0.703);
  width: 100vw;
  margin-left: -125px;
  height: 50px;
}

.input{
  background-color: white;
  border-radius: 6px;
}

.btn{
  border-radius: 4px;
  background-color: whitesmoke;
  color: black;
}
.btn:hover{
  background-color: black;
  color: whitesmoke
}

</style>
