<template>
  <div>
      <AppAlert>
         <!-- Header & Navbar -->
          <HeaderComponent />
    <!-- Hero or Showcase Section -->
    <section class="hero d-flex flex-column align-items-center justify-content-center">
      <div class="text-center">
        <h1 class="h1 text-white fw-medium fst-italic">Abdelhmed Mgazy</h1>
        <h2 class="display-3 text-white fw-bold">Full-Stack developer <br /> Laravel-Vue.js</h2>
        <a href="#skills" class="btn btn-lg fs-6 fw-medium mt-5 btn-primary p-3">TELL ME MORE</a>
      </div>
    </section>
    
    <!-- Skills Section -->
      <Skills />
    <!-- Portfolio Section -->
    <Portfolio />

    <!-- About Section -->
    <About />

    <!-- Curriculum Vitae Section -->
      <curriculum></curriculum>

     <!-- Contact Section -->
    
      <Contact />
    
    
      </AppAlert>
    </div>
</template>
<script>
import Curriculum from '~/components/Curriculum.vue';
</script>