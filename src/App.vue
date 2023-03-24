<template>
  <div>
    <Background/>
    <Header></Header>
    <router-view></router-view>
  </div>
</template>

<script>
import Background from "@/components/Background";
import Header from "@/components/Header";
export default {
  name: 'App',
  components:{
    Header,
    Background,
  }
}
</script>

<style>
#app {
@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600;700&display=swap");
  font-family: "Montserrat", sans-serif;
}

body {
  margin: auto;
}

</style>