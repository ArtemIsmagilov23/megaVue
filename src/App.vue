<script setup>
import { ref } from 'vue';
import counter from './counter.vue';
import products from './products.vue';

console.log()


let buyPaiment = () =>{
    let myMoney = $store.state.money
    let myPrice = $store.state.price;
if(myMoney >= myPrice){
    myMoney - myPrice
}
}

</script>

<template>
 <div class="container">

<counter />
<h2 class="money">balance: {{$store.state.money}}</h2>
<button class="btnBuy" @click="buyPaiment">buy</button>
<products />
 </div>
</template>

<style scoped>

</style>
