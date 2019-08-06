<template>
    <div id="profile">
        <h2 class="content-title font-weight-regular mt-4 ml-4">
            <v-icon>mdi-account-circle-outline</v-icon>
            Profile
        </h2>
        <v-layout wrap align-center>
            <v-flex sm6 xs12>
                <v-layout justify-center>
                <img 
                    src="../assets/profile-image.png" 
                    alt="Profile Image"
                    class="ma-5"
                    width="300"
                    height="300"
                >
                </v-layout>
            </v-flex>
            <v-flex sm6 xs12>
                <p class="text ma-5">
                    はじめまして、データエンジニアとフルスタックエンジニアとして活動しているヤマモトコウヘイと申します。
                    <br>
                    漠然と自然科学系に進みたかったものの一浪の末受験に失敗し、神戸大学の情報系学科に進学。
                    大学生時代を勉強に費やすも学科主席は取れずに次席で卒業。同大学院に進学。
                    <br>
                    大学院在学中はスーパーコンピュータでの磁気流体運動のシミュレーション計算、大規模データの可視化を研究。
                    また、ブラウン大学との共同研究、ソフトウェア会社でのSNSアプリ開発、カナダへの留学（人工知能についての研究）、不動産テック会社でのデータ分析とWebアプリ開発など幅広い経験の機会に恵まれる。
                    卒業後はカナダのトロントへ渡航。
                    <br>
                    トロントでソフトウェアエンジニアとしての職を探すも実務経験不足で約150社に落ちる。ビジネスネットワーキングパーティで出会ったスタートアップ企業のCEOに誘われ、メンバーの一員になる。
                    <br>
                    現在トロントのスタートアップ企業にて役員に在任中。
                </p>
            </v-flex>
        </v-layout>
    </div>
</template>

<script>
export default {
    name: 'Profile',
    data: () => {
        return {
            text: `
                はじめまして、データエンジニアとフルスタックエンジニアとして活動しているヤマモトコウヘイと申します。
                漠然と自然科学系に進みたかったものの一浪の末受験に失敗し、神戸大学の情報系学科に進学。華の大学生時代を勉強に費やすも学科主席は取れずに次席で卒業。
                現在トロントのスタートアップ企業にて役員に在任中。
            `
        }
    }
}
</script>

<style scoped>
#profile {
    padding: auto;
    /* height: 500px; */
}

.text {
    /* white-space: pre-wrap; */
    word-wrap:break-word;
}
</style>

