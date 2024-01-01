<template>
  <div>

    <NavPage/>
    <WelcomePage/>
    <DescriptionsPage/>
    <BlogsPage/>
    <SearchForm/>
    <!-- <FooterPage/> -->
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
  </div>
</template>

<script>
import NavPage from './components/NavPage.vue'
import WelcomePage from './components/WelcomePage.vue'
import DescriptionsPage from './components/DescriptionsPage.vue'
import BlogsPage from './components/BlogsPage.vue'
import FooterPage from './components/FooterPage.vue'
import SearchForm from './components/SearchForm.vue'
export default {
  name: 'App',
  components: {
    NavPage, WelcomePage,DescriptionsPage,BlogsPage, FooterPage, SearchForm
  }
}
</script>

<style>

@font-face{
  font-family:"Montserrat";
  src:url('./assets/fonts/Montserrat-Regular.ttf');
}

@font-face{
  font-family:"OpenSans";
  src:url('./assets/fonts/OpenSans-Regular.ttf');
}

@font-face{
  font-family:"Roboto";
  src:url('./assets/fonts/Roboto-Regular.ttf');
}

:root{
  --primary: #132d5b;
  --secondary: #2277d0;
  --tertiary:#e1ecfd;
  --foreground: black;
  --background: white;
  --light-grey: rgb(184, 184, 184);
  --dark-grey: grey;
  --faint-white:rgba(255, 255, 255, 0.418);
  --faint-white-two:rgba(255, 255, 255, 0.801);
  --faint-black:rgba(0, 0, 0, 0.623);
  --faint-primary:#132d5bd5;
  --blur:blur(4px);
  --primary-font:Roboto;
  --secondary-font:OpenSans;
  --logo-font:Montserrat;
}

body{
  margin:0;
}
</style>
