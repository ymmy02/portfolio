<template>
  <v-flex md6 sm12>
    <v-hover v-slot:default="{ hover }">
        <v-card
            height="250"
            class="ma-3 brown lighten-5"
            :elevation="hover ? 12 : 2"
            outlined
        >
            <v-list-item three-line>
            <v-list-item-content>
                <v-list-item-title class="headline mb-1">{{ title }}</v-list-item-title>
                <div class="text-xs-center">{{ content }}</div>
            </v-list-item-content>
            </v-list-item>

            <v-layout align-center justify-center>
                <v-img
                    v-for="image in images"
                    :key="image.index"
                    :src="image"
                    :lazy-src="image"
                    class="mx-5"
                    max-width="100"
                    height="auto"
                ></v-img>
            </v-layout>
        </v-card>
    </v-hover>
  </v-flex>
</template>

<script>
export default {
    name: 'SkillCard',
    props: {
        title: String,
        content: String,
        images: Array
    },
}
</script>

