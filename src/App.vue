<template>
  <div id="app">
    <Header />
    Food delivery
    <Footer />
  </div>
</template>

<script>
import Header from "@/components/Header";
import Footer from "@/components/Footer";

export default {
  name: "App",
  components: { Header, Footer },
};
</script>

<style>
* {
  font-family: "Source Sans Pro";
}
</style>
