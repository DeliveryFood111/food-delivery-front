<template>
  <div id="app">
    <Header />
    <MainScreen />
    <Benefits />
    <HistoryWithImages />
    <Menu />
    <PopularProducts />
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
import PopularProducts from "@/components/PopularProducts";
import Menu from "@/components/Menu";

export default {
  name: "App",
  components: {
    Menu,
    Benefits,
    Header,
    Footer,
    MainScreen,
    HistoryWithImages,
    BenefitsEnd,
    PopularProducts,
  },
};
</script>

<style>
* {
  font-family: "Source Sans Pro";
}
</style>
