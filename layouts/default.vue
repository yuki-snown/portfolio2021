<template>
  <v-app dark>
    <v-navigation-drawer app>
      <v-img
        src="https://pbs.twimg.com/profile_images/1226786060186746880/KZW4E8XQ_400x400.jpg"
        class="pa-7 rounded-circle"
        max-width="15vw"
        max-height="15vw"
      ></v-img>
      <v-list>
        <v-list-item v-for="item in items" :key="item.title" :to="item.to" link>
          <v-list-item-icon>
            <v-icon>{{item.icon}}</v-icon>
          </v-list-item-icon>
          <v-list-item-content>
            <v-list-item-title>
              {{item.title}}
            </v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-app-bar app>
      <v-text to="/">
        <h1>{{title}}</h1>
      </v-text>
    </v-app-bar>

    <v-main>
      <v-container fluid>
        <router-view></router-view>
      </v-container>
        <v-btn
          dark
          fixed
          bottom
          right
          fab
          x-large
          to="/"
        >
          <v-icon>mdi-apps</v-icon>
        </v-btn>
    </v-main>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-account',
          title: 'I am',
          to: '/introduce'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Skill',
          to: '/skill'
        },
        {
          icon: 'mdi-database',
          title: 'History',
          to: '/history'
        },
        {
          icon: 'mdi-github',
          title: 'Github',
          to: '/github'
        }
      ],
      title: "yu-ki's PortFolio"
    }
  }
}
</script>
