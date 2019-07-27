<template>
    <v-layout align-center justify-center>
        <div class="title">
            <v-img
            src="../assets/title-logo.png"
            lazy-src="../assets/title-logo.png"
            max-width="500"
            max-height="300"
            ></v-img>
        </div>
  </v-layout>
</template>

<script>
export default {
    name: "TitleLogo",
    data:() => {
        return {
        }
    }
}
</script>

<style scoped>
.title {
    height: 500px;
    padding-top: 200px;
}
</style>

