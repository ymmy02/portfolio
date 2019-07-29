<template>
    <div class="hobby">
        <h2 class="content-title font-weight-regular mt-4 ml-4">
            <v-icon>mdi-heart-outline</v-icon>
            Hobby
        </h2>
        <HobbyItem 
            v-for="item in items"
            :key="item.title"
            :icon="item.icon"
            :title="item.title"
            :comment="item.comment"
            :image="item.image"
        />
    </div>
</template>

<script>
import HobbyItem from './HobbyItem';

export default {
    name: 'Hobby',
    components: {
        HobbyItem
    },
    data: () => ({
        items: [
            {
                icon: 'mdi-karate',
                title: '合気道',
                comment: '週二回',
                image: require('../assets/hobby/aikido.png'),
            },
            {
                icon: 'mdi-apple-safari',
                title: '旅行',
                comment: '週二回',
                image: require('../assets/hobby/travel.jpg'),
            },
            {
                icon: 'mdi-beer',
                title: 'ビール',
                comment: '週二回',
                image: require('../assets/hobby/beer.jpg'),
            },
            {
                icon: 'mdi-chart-line',
                title: '投資',
                comment: '週二回',
                image: require('../assets/hobby/investment.png'),
            },
        ]
    })
}
</script>
