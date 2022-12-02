<script lang="js">
import Header from './components/Header.vue';
import Logo from "./components/Logo.vue";
import Form from "./components/Form.vue";
import Section from "./components/Section.vue";
import Footer from "./components/Footer.vue";
import DemoImg from './components/DemoImg.vue';
import SocialMedia from './components/SocialMedia.vue';
import { FaBandsFacebookF } from "@kalimahapps/vue-icons/fa";
import { BsTwitter } from "@kalimahapps/vue-icons/bs";
import { BsInstagram } from "@kalimahapps/vue-icons/bs";
export default {
components:{ Header, Logo, Form, Section, Footer, DemoImg, FaBandsFacebookF, SocialMedia, BsTwitter, BsInstagram},
data(){
  return {

  }
}
};
</script>

<template>
  <div></div>
  <div class="text-center font-libreFranklin text-xl py-10">
    <Logo />
    <Header />
    <Form />
    <DemoImg />
   
    <!-- to be continued -->
    <SocialMedia>
      <FaBandsFacebookF />
      <BsTwitter />
      <BsInstagram />
    </SocialMedia>
    <!-- -->
   
    <Section />
  </div>
  <Footer />
</template>

<style scoped></style>
