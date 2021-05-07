<template>
  <div class="users container">
    <h1>Información de usuario</h1>

    <router-link 
      :to='{ name: "Users", params: { id: item } }' 
      v-for='(item, index) of userArray' 
      :key="index">
      <button>{{item}}</button>
    </router-link>

    <User />
  </div>
</template>

<script>
import User from '@/components/User.vue'

export default {
  components: {
    User
  },
  data(){
    return {
      userArray: [
        'Vargas',
        'Carlos',
        'Paola'
      ]
    }
  }
}
</script>
