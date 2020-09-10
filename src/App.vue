<template>
  <v-app>
    <v-main>
      <router-view />
    </v-main>
    <Footer />
  </v-app>
</template>

<script>
import Footer from "@/components/Footer.vue";

export default {
  name: "App",

  components: {
    Footer
  },

  data: () => ({
    //
  })
};
</script>

<style>
.hero {
  background: linear-gradient(rgba(0, 0, 0, 0.4), rgba(0, 0, 0, 0.8)),
    url("https://www.zerorezsavannah.com/wp-content/uploads/air-duct-cleaning.jpg");
  margin-top: -4em;
  padding-top: 10em;
  padding-bottom: 6em;
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}
html {
  scroll-behavior: smooth;
}
body {
  font-family: "Open Sans", sans-serif;
}
h1,
h2,
h3,
h4,
h5 {
  font-family: "Montserrat", sans-serif;
  font-weight: 900;
}
.intro {
  padding-top: 6em;
}
.intro h5 {
  text-transform: uppercase;
}
.upper-border {
  border-top: solid #333;
}
.upper-border-white {
  border-top: solid #fff;
}

#services {
  padding-top: 2em;
}

@media only screen and (max-width: 960px) {
  .left-img {
    display: none;
  }
}
</style>
