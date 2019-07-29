<template>
    <div class="ma-4">
        <h3 class="ml-5 fonto-weight-regular">
            <v-icon>{{ icon }}</v-icon>
            {{ title }}
        </h3>
        <v-layout align-center justify-space-around>
            <p>{{ comment }}</p>
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

