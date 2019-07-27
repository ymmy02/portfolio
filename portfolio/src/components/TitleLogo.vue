<template>
    <v-layout align-center justify-center>
    <v-img
      src="../assets/title-logo.png"
      lazy-src="../assets/title-logo.png"
      max-width="500"
      max-height="300"
    ></v-img>
  </v-layout>
</template>

<script>
export default {
    name: "TitleLogo",
    data:() => {
        return {
            logo: require('@/assets/title-logo.png'),
        }
    }
}
</script>

