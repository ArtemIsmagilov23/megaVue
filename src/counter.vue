<template>


<button @click="increse" class="btn btn success">+money</button>
</template>

<script>

export default {
methods:{
increse(){
this.$store.state.money = this.$store.state.money + 500
}
}
}
</script>

