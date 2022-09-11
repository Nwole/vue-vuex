<template>
  <div>
    <p class="text-xl text-green-600">counter is : {{doubleCounter}}</p>
    <p>Number of Clicks: {{stringCounter}}</p>
  </div>
</template>

<script>
  import { mapGetters } from 'vuex';
export default {
computed:{ 
  ...mapGetters([
  'doubleCounter',
  'stringCounter'
])
}
}
</script>

<style>

</style>