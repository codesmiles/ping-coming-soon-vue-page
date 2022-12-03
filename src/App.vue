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

    <!-- NEED A BETTER LOGIC -->
    <div class="flex justify-center md:mt-20">
      <SocialMedia>
        <a href="https://www.facebook.com/codesmiles" aria-label="Facebook">
          <FaBandsFacebookF />
        </a>
      </SocialMedia>
      <social-media>
        <a href="https://www.twitter.com/codesmiles_" aria-label="Twitter">
          <BsTwitter />
        </a>
      </social-media>
      <social-media>
        <a href="https.//www.instagram.com/codesmiles" aria-label="instagram">
          <BsInstagram />
        </a>
      </social-media>
    </div>
    <!--FIND A BETTER WAY TO MAKE THIS WORK -->

    <Section />
  </div>
  <Footer />
</template>

<style scoped></style>
