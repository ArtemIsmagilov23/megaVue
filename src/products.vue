<script>
function grob(){
alert("123")
}
export default {
    methods:{
newMoney(){
this.$store.state.money - this.$store.state.price
}}
};

</script>

<template>
  <div class="oneProduct">
    <img
      class="boot"
      src="https://krostore.ru/images/product/l/5395-nike-air-force-1-lv8-whitered-f22fb.jpg"
      alt="тут фотка крутая"
    />
    <h2 class="priceOneBoot">{{ $store.state.price }} <sup>rub</sup></h2>
    
</div>
<button @click="grob">dfgdfgfd</button>
 
</template>

<style>
.boot {
  width: 512px;
  height: 352px;
  position: absolute;
}
.oneProduct {
  border: 1px solid gray;
  width: 600px;
  height: 600px;
}
.priceOneBoot {
  margin-top: 400px;
  position: absolute;
  margin-left: 200px;
}
.btnBuy {
  position: absolute;
  margin-top: 450px;
  margin-left: 200px;
}
</style>
