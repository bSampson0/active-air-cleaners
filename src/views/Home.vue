<template>
  <div class="home">
    <Navigation />
    <Hero />
    <Services />
    <Contact />
  </div>
</template>

<script>
// @ is an alias to /src
import Navigation from "@/components/Navigation.vue";
import Hero from "@/components/Hero.vue";
import Services from "@/components/Services.vue";
import Contact from "@/components/Contact.vue";

export default {
  name: "Home",
  components: {
    Navigation,
    Hero,
    Services,
    Contact
  }
};
</script>
