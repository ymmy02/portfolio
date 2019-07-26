<template>
  <v-app>
    <NavBar />
    <v-content>
      <Profile />
    </v-content>
    <v-content>
      <Skill />
    </v-content>
    <v-content>
      <Hobby />
    </v-content>
  </v-app>
</template>

<script>
import NavBar from './components/NavBar';
import Profile from './components/Profile';
import Skill from './components/Skill';
import Hobby from './components/Hobby';

export default {
  name: 'App',
  components: {
    NavBar,
    Profile,
    Skill,
    Hobby
  },
  data: () => ({
    //
  }),
};
</script>
