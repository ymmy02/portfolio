<template>
    <div class="ma-5">
        <h3 class="ml-5 fonto-weight-regular">
            <v-icon>{{ icon }}</v-icon>
            {{ title }}
        </h3>
        <v-layout align-center justify-space-around>
            <p class="comment">{{ comment }}</p>
            <v-img
                :src="image"
                :lazy-src="image"
                class="mx-5"
                max-width="250"
                height="auto"
            ></v-img>
        </v-layout>
    </div>
</template>

<script>
export default {
    name: 'HobbyItem',
    props: {
        icon: String,
        title: String,
        comment: String,
        image: String
    }
}
</script>

<style scoped>
.comment {
    white-space: pre-wrap;
    word-wrap:break-word;
}
</style>

