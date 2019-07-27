<template>
    <div class="profile">
        <h2 class="content-title font-weight-regular mt-4 ml-4">
            <v-icon>mdi-account-circle-outline</v-icon>
            Profile
        </h2>
        <v-layout align-center justify-center>
            <p class="text">{{ text }}</p>
        </v-layout>
    </div>
</template>

<script>
export default {
    name: 'Profile',
    data: () => {
        return {
            text: `
                こんにちは
                はじめまして
                山本と言います。
            `
        }
    }
}
</script>

<style scoped>
.profile {
    padding: auto;
    /* height: 500px; */
}

.text {
    white-space: pre-wrap;
    word-wrap:break-word;
}
</style>

