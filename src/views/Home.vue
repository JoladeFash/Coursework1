<template>
 <header class="masthead bg-primary text-white text-center">
    <div class="container d-flex align-items-center flex-column">

      <!-- Masthead Avatar Image -->
      <img class="masthead-avatar mb-5" src="img/avataaars.svg" alt="">

      <!-- Masthead Heading -->
      <h1 class="masthead-heading text-uppercase mb-0">Welcome!</h1>

      <!-- Icon Divider -->
      <div class="divider-custom divider-light">
        <div class="divider-custom-line"></div>
        <div class="divider-custom-icon">
          <i class="fas fa-star"></i>
        </div>
        <div class="divider-custom-line"></div>
      </div>
      <router-link class="btn btn-primary btn-lg" to="/signup" role="button">Sign up</router-link>

      <!-- Masthead Subheading -->
      <p class="masthead-subheading font-weight-light mb-0">Find After School Activities for Students</p>

    </div>
  </header>





  <!-- <div class="jumbotron">
    <div class="container">
      <h1 class="display-4">Welcome!</h1>
      <p class="lead">You can choose Extra Curricular Activities and Courses</p>
      <hr class="my-4">
      <p>Trying to stay at the top? Register with us and get access to a wide range os extra curricluar activities and courses.</p>
      <router-link class="btn btn-primary btn-lg" to="/signup" role="button">Sign up</router-link>
    </div>
  </div> -->
</template>
<script>
export default {
  filterResutl(){

  }
}
</script>

