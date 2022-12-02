<script lang="js">
import Header from './components/Header.vue';
import Logo from "./components/Logo.vue";
import Form from "./components/Form.vue";
import Section from "./components/Section.vue";
import Footer from "./components/Footer.vue";
import DemoImg from './components/DemoImg.vue';
export default {
components:{ Header, Logo, Form, Section, Footer, DemoImg },
data(){
  return {
    source:"src\assets\images\illustration-dashboard.png"
  }
}
};
</script>

<template>
  <div class="text-center font-libreFranklin text-xl py-10">
    <!-- <font-awesome-icon icon="fa-brands fa-facebook" />
    <font-awesome-icon icon="fa-brands fa-twitter" />
    <font-awesome-icon icon="fa-brands fa-instagram" /> -->
    <Logo />
    <Header />
    <Form />
    <DemoImg />
    <Section />
  </div>

  <Footer />
</template>

<style scoped></style>
