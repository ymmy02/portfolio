<template>
  <v-footer
    color="brown lighten-5"
    padless
  >
    <v-layout
      justify-center
      wrap
    >
      <v-btn icon href="#profile" 
      v-smooth-scroll="{ duration: 500, offset: 0, container: '' }">
          <v-icon>mdi-account-circle-outline</v-icon>
      </v-btn>
      <v-btn icon href="#skill"
      v-smooth-scroll="{ duration: 500, offset: 0, container: '' }">
          <v-icon>mdi-laptop</v-icon>
      </v-btn>
      <v-btn icon href="#hobby"
      v-smooth-scroll="{ duration: 500, offset: 0, container: '' }">
          <v-icon>mdi-heart-outline</v-icon>
      </v-btn>
      <v-btn href="https://github.com/ymmy02" icon>
          <v-icon>mdi-github-circle</v-icon>
      </v-btn>
      <v-btn href="https://www.linkedin.com/in/kohei-yamamoto-a12557158/" icon>
          <v-icon>mdi-linkedin-box</v-icon>
      </v-btn>
      <v-flex
        lighten-2
        py-4
        text-center
        xs12
      >
        {{ new Date().getFullYear() }}
      </v-flex>
    </v-layout>
  </v-footer>
</template>

<script>
  export default {
    data: () => ({
      links: [
        'Home',
        'About Us',
        'Team',
        'Services',
        'Blog',
        'Contact Us',
      ],
    }),
  }
</script>
