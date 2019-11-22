<template>
  <!--<div id="nav" class="nav">
    <router-link to="/" class="brand">Real World Events</router-link>
    <nav>
      <router-link :to="{ name: 'event-list' }">List</router-link> |
      <router-link :to="{ name: 'event-create' }">Create</router-link>
    </nav>
  </div>-->
 <nav class="navbar navbar-expand-lg bg-secondary text-uppercase fixed-top" id="mainNav">
    <div class="container">
      <router-link class="navbar-brand js-scroll-trigger" to="/">Find Courses</router-link>
      <button class="navbar-toggler navbar-toggler-right text-uppercase font-weight-bold bg-primary text-white rounded" type="button" data-toggle="collapse" data-target="#navbarResponsive" aria-controls="navbarResponsive" aria-expanded="false" aria-label="Toggle navigation">
        Menu
        <i class="fas fa-bars"></i>
      </button>
      <div class="collapse navbar-collapse" id="navbarResponsive">
        <ul class="navbar-nav ml-auto">
          <li class="nav-item mx-0 mx-lg-1">
               <router-link class="nav-link py-3 px-0 px-lg-3 rounded js-scroll-trigger" to="/">Home</router-link>
            
          </li>
          <li class="nav-item mx-0 mx-lg-1">
            <a style="cursor: pointer" v-if="isAuth"  class="nav-link" @click="logout">Logout</a>
            
            <router-link v-else class="nav-link" to="/signup">Login</router-link>
          </li>
        </ul>
      </div>
    </div>
  </nav>


         
</template>

<script>
  import {mapGetters} from 'vuex'
  
    export default {
        computed:{
          isAuth(){
            return this.$store.getters.isAuth;
          }
        },
      methods:{
        logout(){
          console.log('lodgout');
          this.$store.commit('UNSET_USER');
          this.$router.push('/');
        }
      }
    }
</script>