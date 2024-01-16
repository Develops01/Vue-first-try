<script setup>
import Hero from "./components/Hero.vue";
import Nav from "./components/Nav.vue";
import About from "./components/About.vue";
import Cards from "./components/Cards.vue";
import Consultation from "./components/Consultation.vue";
import Consultation2 from "./components/Consultation2.vue";
import Footer from "./components/Footer.vue";
import Form from "./components/Form.vue";
import RoadMap from "./components/RoadMap.vue";
import Statics from "./components/Statics.vue";
</script>

<template>
  <Nav />
  <div class="absolute top-0 -z-10 w-full h-[25rem] bg-[#BD6678]"></div>
  <Hero />
  <About />
  <Cards />
  <Statics />
  <Consultation />
  <RoadMap />
  <Consultation2 />
  <Form />
  <Footer />
</template>

<style scoped></style>
