<template>
    <div id="hobby">
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
                comment: `
                    週に２〜３回ほど合気道の稽古に参加している。
                    心身の健康にかなり貢献している。
                    稽古で汗をかいた後のビールは最高に美味しい。
                    合気道を通した人との交流も楽しみの一つ
                `,
                image: require('../assets/hobby/aikido.png'),
            },
            {
                icon: 'mdi-book-open-page-variant',
                title: '読書',
                comment: `
                    移動時間に読書をするのが好き。
                    最近Kindleを購入してかなり読書が捗っている。
                    読むジャンルはバラバラ。
                    出来るだけ自分と遠いカテゴリーを読むのを心がけている。
                `,
                image: require('../assets/hobby/reading.png'),
            },
            {
                icon: 'mdi-apple-safari',
                title: '旅行',
                comment: `
                    普段はインドア派なのになぜか海外に行くことが多い。
                    国内では城崎温泉がお気に入りで最低年に一回は訪れる。
                    右の写真はポルトガルのポルトにて
                `,
                image: require('../assets/hobby/travel.jpg'),
            },
            {
                icon: 'mdi-beer',
                title: 'ビール',
                comment: `
                    IPAビールが好物。
                    カナダはビールの種類が非常に多く、ビール好きには天国。 
                    最近は日本にもIPA含めクラフトビールが増えてきて嬉しい。。
                `,
                image: require('../assets/hobby/beer.jpg'),
            },
            {
                icon: 'mdi-chart-line',
                title: '投資',
                comment: `
                    資産形成を目指して株、FXを勉強中。
                    値動きに対する自分の気持ちの思わぬ動き方がかなり面白い。
                    データ解析や機械学習を活かそうとしているもののなかなか難しい...。
                `,
                image: require('../assets/hobby/investment.png'),
            },
        ]
    })
}
</script>
