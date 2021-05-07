<template>
  <div class="home container">
    <HelloWorld msg="Bienvenido a Vue.js App con rutas"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>
