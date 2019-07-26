<template>
  <div>
    <v-toolbar
      :extended="extended"
      :prominent="prominent"
      :dense="dense"
      :collapse="collapse"
      :flat="flat"
      :src="bg ? background : undefined"
      :extension-height="extensionHeight"
    >
      <v-toolbar-title>Kohei Yamamoto's Portfolio</v-toolbar-title>

      <v-spacer></v-spacer>

      <v-toolbar-items>
        <v-btn text>
            <v-icon>mdi-account-circle-outline</v-icon>
            Profile
        </v-btn>
        <v-btn text>
            <v-icon>mdi-laptop</v-icon>
            Skill
        </v-btn>
        <v-btn text>
            <v-icon>mdi-heart-outline</v-icon>
            Hobby
        </v-btn>
        <v-btn href="https://github.com/ymmy02" icon>
            <v-icon>mdi-github-circle</v-icon>
        </v-btn>
      </v-toolbar-items>
    </v-toolbar>
  </div>
</template>

<script>
  export default {
    name: 'NavBar',
    data: () => ({
      extended: false,
      extendedSlot: false,
      prominent: false,
      dense: false,
      collapse: false,
      flat: true,
      bg: true,
      extensionHeight: 48,
      background: require('@/assets/navbar-background.jpg')
    }),
  }
</script>
