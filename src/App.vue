<template>
<div class="app">
  <p>{{ name }} - {{  age }}</p>
  <button @click="changeName('yoyo')">Change name</button>
  <button @click="changeAge('30')">Change age</button>
</div>
</template>

<script lang="ts">

import { defineComponent } from 'vue';

// let age :string|number

export default defineComponent({
  name: 'App',
  components: { },
  data(){
    return {
      name:'ali',
      age:52 as number|string
    }
  },
  methods:{
    changeName(name:string)
    {
      this.name=name;
    },
    changeAge(age : number|string){
       this.age=age;
    }
  }
});
</script>

<style>

</style>
