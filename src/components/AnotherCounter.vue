<template>
    <div class="pt-10">
      <button class="btn-btn" @click="increment">Increment</button>
      <button class="btn-btn" @click="decrement">Decrement</button>
    </div>
  </template>
  
  <script>
    import { mapMutations, mapActions } from 'vuex';
  export default {
    dada() {
      return {};
    },
    // methods: {
    //     ...mapMutations([
    //     'increment',
    //     'decrement'
    // ])
    // },
    methods: {
        ...mapActions([
        'increment',
        'decrement'
    ])
    }
   
  };
  </script>
  
  <style scoped>
  .btn-btn {
    color: white;
    font-size: 18px;
    font-weight: bold;
    margin-left: 5px;
    border-radius: 8px;
    background: blue;
    padding: 10px;
  }
  .btn-btn:hover {
    background-color: lightgray;
  }
  </style>
  