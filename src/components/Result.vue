<template>
  <div>
    <p class="text-xl text-green-600">counter is : {{counter}}</p>
  </div>
</template>

<script>
export default {
computed: {
    counter(){
       return this.$store.getters.doubleCounter;
    }
}
}
</script>

<style>

</style>