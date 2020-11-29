<template>
  <div id="app">
    <List/>
    <Footer/>
  </div>
</template>

<script>
import List from './components/List'
import Footer from './components/Footer'

export default {
  name: 'App',
  components: {
    List,
    Footer
  }
}
</script>

<style>
@import url(https://fonts.googleapis.com/css?family=Noto+Sans+JP:100,200,300,400,500,600,700,800,900);
@import url(https://fonts.googleapis.com/css?family=Poppins:100,200,300,400,500,600,700,800,900);
@import url(https://fonts.googleapis.com/css?family=Ubuntu+Mono:100,200,300,400,500,600,700,800,900);
</style>
