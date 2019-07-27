<template>
  <v-app>
    <NavBar />
    <v-content class="grey lighten-4">
      <TitleLogo />
    </v-content>
    <v-content id="profile" class="grey lighten-5">
      <Profile />
    </v-content>
    <v-content id="skill" class="grey lighten-5">
      <Skill />
    </v-content>
    <v-content id="hobby" class="grey lighten-5">
      <Hobby />
    </v-content>
  </v-app>
</template>

<script>
import NavBar from './components/NavBar';
import TitleLogo from './components/TitleLogo';
import Profile from './components/Profile';
import Skill from './components/Skill';
import Hobby from './components/Hobby';

export default {
  name: 'App',
  components: {
    NavBar,
    TitleLogo,
    Profile,
    Skill,
    Hobby
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

