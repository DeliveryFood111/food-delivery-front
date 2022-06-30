<template>
  <div id="app">
    <Header />
    <Footer />
    <Benefits />
  </div>
</template>

<script>
import Benefits from "@/components/Benefits";
import Header from "@/components/Header";
import Footer from "@/components/Footer";

export default {
  name: "App",
  components: { Benefits, Header, Footer }
};
</script>

<style>
* {
  font-family: "Source Sans Pro";
}
</style>
