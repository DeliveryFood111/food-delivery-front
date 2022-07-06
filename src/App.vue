<template>
  <div id="app">
    <Header />
    <MainScreen />
    <Benefits />
    <HistoryWithImages />
    <Footer />
  </div>
</template>

<script>
import Benefits from "@/components/Benefits";
import Header from "@/components/Header";
import Footer from "@/components/Footer";
import MainScreen from "@/components/MainScreen";
import HistoryWithImages from "@/components/HistoryWithImages";

export default {
  name: "App",
  components: { Benefits, Header, Footer , MainScreen, HistoryWithImages }
};
</script>

<style>
* {
  font-family: "Source Sans Pro";
};
</style>
