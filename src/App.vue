<script setup lang="ts">
import { ref } from 'vue';
import { RouterLink, RouterView } from 'vue-router'
import router from './router'

// types 
type localhost = string


// constants 
const localhost = ref(window.localStorage.access)


// logic 
function start() {
  if(localhost.value === undefined){
    router.push('/auth')
  }
}
start()



</script>

<template>

  <RouterView />
</template>

<style>

</style>
