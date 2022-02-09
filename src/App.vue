<template>
  <div id="app">
   <Header />
   <Content />
   <Info />
   <Footer />

  </div>
</template>

<script>
 import Header from './components/Header.vue'; 
 import Content from './components/Content.vue'; 
 import Info from './components/Info.vue'; 
 import Footer from './components/Footer.vue'; 
 

export default {
  name: 'App',
  components: {
  Header,
  Content,
  Info,
  Footer
  }
}
</script>

<style lang="scss">

@import "./assets/scss/index.scss";

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;

  body
  {
    padding: 80px 0;
    background-color: black;
    height: 100vh;
    font-family: $segoe-bold; 
  }
}

</style>
