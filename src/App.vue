<template>
  <div id="app">
    <Header />
    <MainScreen />
    <Benefits />
    <Footer />
  </div>
</template>

<script>
import Benefits from "@/components/Benefits";
import Header from "@/components/Header";
import Footer from "@/components/Footer";
import MainScreen from "@/components/MainScreen";

export default {
  name: "App",
  components: { Benefits, Header, Footer, MainScreen }
};
</script>

<style>
* {
  font-family: "Source Sans Pro";
}
</style>
