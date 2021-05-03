<template>
  <v-timeline>
    <v-timeline-item v-for="item in items" :key="item" color='white'>
        <v-card>
            <v-card-title class="text-h5 bold">
                {{item.date}} / {{item.title}}
            </v-card-title>
            <v-card-text class="text-h5 mb-2 white--text text-center">
                {{item.text}}
            </v-card-text>
        </v-card>
    </v-timeline-item>
  </v-timeline>
</template>

<script>
export default {
    data() {
        return {
            items: [
                {
                    date: '2019.07 - 現在',
                    title: 'Phoxter',
                    text: '機械学習プロダクトの開発'
                },
                {
                    date: '2019.11',
                    title: "PwC's Cyber Security Hackathon",
                    text: 'セキュリティの脆弱性調査'
                },
                {
                    date: '2020.02',
                    title: 'mixi bug shooting challenge',
                    text: 'プロダクトのバグの調査'
                },
                {
                    date: '2020.02',
                    title: 'NISCON',
                    text: 'NTT.comのISUCON'
                },
                {
                    date: '2020.02',
                    title: 'CA tech Challenge 2222ハッカソン!!',
                    text: 'お年玉企画の運営サービスを開発'
                },
                {
                    date: '2020.03',
                    title: 'Recruit Speed Hackathon',
                    text: 'フロントのパフォーマンスチューニング'
                },
                {
                    date: '2020.03',
                    title: 'ドワンゴ　就業型インターンシップ',
                    text: 'Androidアプリ開発'
                },
                {
                    date: '2020.08',
                    title: 'チームラボ　サマーインターン',
                    text: 'ECサイトのサーバサイド開発'
                },
                {
                    date: '2020.09',
                    title: 'CA 分析型インターンシップ',
                    text: 'アドテクの予測モデルを作成'
                },
                {
                    date: '2020.09 - 現在',
                    title: 'マネーフォワード　就業型インターン',
                    text: '機械学習モデルの作成'
                },
                {
                    date: '2020.10',
                    title: 'mixi TDD challenge',
                    text: 'テスト開発駆動のワークショップ'
                },
                {
                    date: '2020.03',
                    title: 'CA ABEMA Grouth Tech',
                    text: 'サーバサイド及び機械学習モデルの開発'
                }
            ]
        }
    }
}
</script>
