<template>
  <Calc/>
  
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import Calc from './components/Calc.vue';

export default defineComponent({
  name: 'App',
  components: {
    Calc
}
});
</script>

<style>

body{
  background-color: #DAF0FF;
}
</style>
