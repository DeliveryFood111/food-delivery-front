<template>
  <div id="app">
    <Header />
    <Benefits />
  </div>
</template>

<script>
import Benefits from "@/components/Benefits";
import Header from "@/components/Header";

export default {
  name: "App",
  components: { Benefits, Header }
};
</script>

<style>
* {
  font-family: "Source Sans Pro";
}
</style>
