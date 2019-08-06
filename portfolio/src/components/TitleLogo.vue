<template>
    <div id="title" class="grey lighten-4">
        <v-layout align-center justify-center>
            <v-img
            src="../assets/title-logo.png"
            lazy-src="../assets/title-logo.png"
            max-width="500"
            max-height="auto"
            ></v-img>
        </v-layout>
    </div>
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
#title {
    width: 100%;
    height: 500px;
    padding-top: 200px;
}
</style>

