<template>
  <div id="app">
    <Header />
    <MainScreen />
    <Benefits />
    <HistoryWithImages />
    <BenefitsEnd />
    <Footer />
  </div>
</template>

<script>
import Benefits from "@/components/Benefits";
import Header from "@/components/Header";
import Footer from "@/components/Footer";
import MainScreen from "@/components/MainScreen";
import HistoryWithImages from "@/components/HistoryWithImages";
import BenefitsEnd from "@/components/BenefitsEnd";

export default {
  name: "App",
  components: {Benefits, Header, Footer, MainScreen, HistoryWithImages, BenefitsEnd}
};
</script>

<style>
* {
  font-family: "Source Sans Pro";
};
</style>
