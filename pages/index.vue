<template>
  <v-container fluid>
    <v-row dense>
      <v-col
        v-for="card in cards"
        :key="card.title"
        :cols="card.flex"
      >
        <v-card :to="card.to">
          <v-img
            :src="card.src"
            class="white--text align-end"
            gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
            height="35vh"
          >
            <v-card-title v-text="card.title" class="text-h4 white--text" ></v-card-title>
          </v-img>
          <v-spacer></v-spacer>
          <v-card-text class="text-h5 mb-2 white--text" v-text="card.text"></v-card-text>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
  export default {
    data: () => ({
      cards: [
        { title: 'I am', text: '自己紹介', src: 'img1.jpg', flex: 6, to: '/introduce' },
        { title: 'Skill', text: '技術', src: 'img2.jpg', flex: 6, to: '/skill' },
        { title: 'History', text: '参加記録', src: 'img3.jpg', flex: 6, to: '/history' },
        { title: 'Github', text: 'github link', src: 'img4.jpg', flex: 6, to: '/github' },
      ],
    }),
  }
</script>
