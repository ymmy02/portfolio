<template>
  <v-app>
    <NavBar />
    <v-content class="grey lighten-5">
      <TitleLogo />
      <Profile />
      <Skill />
      <Hobby />
    </v-content>
    <Footer />
  </v-app>
</template>

<script>
import NavBar from './components/NavBar';
import TitleLogo from './components/TitleLogo';
import Profile from './components/Profile';
import Skill from './components/Skill';
import Hobby from './components/Hobby';
import Footer from './components/Footer';

export default {
  name: 'App',
  components: {
    NavBar,
    TitleLogo,
    Profile,
    Skill,
    Hobby,
    Footer
  },
  data: () => ({
    //
  }),
};
</script>

<style scoped>
.contents {
  /* background-color: #fff9f5, */
  background-color: black,
}
</style>

