<template>
  <nav>
    <v-toolbar app flat
      :src="bg ? background : undefined"
      :extension-height="extensionHeight"
    >
      <v-toolbar-title>Kohei Yamamoto's Portfolio</v-toolbar-title>

      <v-spacer></v-spacer>

      <v-toolbar-items class="hidden-xs-only">
        <v-btn text href="#profile" 
        v-smooth-scroll="{ duration: 500, offset: 0, container: '' }">
            <v-icon>mdi-account-circle-outline</v-icon>
            Profile
        </v-btn>
        <v-btn text href="#skill"
        v-smooth-scroll="{ duration: 500, offset: 0, container: '' }">
            <v-icon>mdi-laptop</v-icon>
            Skill
        </v-btn>
        <v-btn text href="#hobby"
        v-smooth-scroll="{ duration: 500, offset: 0, container: '' }">
            <v-icon>mdi-heart-outline</v-icon>
            Hobby
        </v-btn>
        <v-btn href="https://github.com/ymmy02" icon>
            <v-icon>mdi-github-circle</v-icon>
        </v-btn>
      </v-toolbar-items>
      <v-app-bar-nav-icon 
        class="hidden-sm-and-up"
        @click="drawer = !drawer"
      ></v-app-bar-nav-icon>
    </v-toolbar>

    <v-navigation-drawer right v-model="drawer" app class="grey lighten-5">
      <v-list dense>
        <v-list-item text href="#profile" 
        v-smooth-scroll="{ duration: 500, offset: 0, container: '' }">
          <v-list-item-icon>
            <v-icon>mdi-account-circle-outline</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>Profile</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

        <v-list-item text href="#skill" 
        v-smooth-scroll="{ duration: 500, offset: 0, container: '' }">
          <v-list-item-icon>
            <v-icon>mdi-laptop</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>Skill</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

        <v-list-item text href="#hobby" 
        v-smooth-scroll="{ duration: 500, offset: 0, container: '' }">
          <v-list-item-icon>
            <v-icon>mdi-heart-outline</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>Hobby</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
  </nav>
</template>

<script>
  export default {
    name: 'NavBar',
    data: () => ({
      bg: true,
      extensionHeight: 48,
      background: require('@/assets/navbar-background.jpg'),
      drawer: false
    }),
  }
</script>
