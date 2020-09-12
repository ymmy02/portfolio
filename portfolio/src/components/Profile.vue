<template>
  <div id="profile">
    <h2 class="content-title font-weight-regular mt-4 ml-4">
      <v-icon>mdi-account-circle-outline</v-icon>Profile
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
          />
        </v-layout>
      </v-flex>
      <v-flex sm6 xs12>
        <p class="text ma-5">
          はじめまして、フリーランスエンジニアとITコンサルタントとして活動している山本晃平と申します。
          <br />大学ではコンピュータサイエンスを専攻し、大学院在学中はスーパーコンピュータでの磁気流体運動のシミュレーション計算、大規模データの可視化を研究。
          また、ブラウン大学との共同研究、ソフトウェア会社でのSNSアプリ開発、カナダへの留学（人工知能についての研究）、不動産テック会社でのデータ分析とWebアプリ開発など幅広い経験の機会に恵まれる。
          卒業後はカナダのトロントへ渡航。
          <br />半年という短期間ながら世界のレベルの高さと厳しさを学ぶ。
          <br />帰国後、フリーランスとして独立し、現在はバックエンドエンジニアとして開発に携わる傍らコンサルタントとして企業のITツール導入のお手伝いをしている。
        </p>
      </v-flex>
    </v-layout>
  </div>
</template>

<style scoped>
#profile {
  padding: auto;
  /* height: 500px; */
}

.text {
  /* white-space: pre-wrap; */
  word-wrap: break-word;
}
</style>

