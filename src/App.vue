<script lang="js">
import Header from './components/Header.vue';
import Logo from "./components/Logo.vue";
import Form from "./components/Form.vue";
import Section from "./components/Section.vue";
import Footer from "./components/Footer.vue";
export default {
components:{ Header,Logo,Form,Section,Footer }
};
</script>

<template>
  <div class="text-center font-libreFranklin text-xl">
  
    <Logo />
    <Header />
    <Form />
    <div class="flex justify-center">
      <img src="src\assets\images\illustration-dashboard.png" alt="illustration dashboard" class="max-w-xl">
    </div>
    <Section />
  
  </div>

  <Footer />
</template>

<style scoped></style>
