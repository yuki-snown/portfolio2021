<template>
  <v-carousel v-model="model" height="90vh">
    <v-carousel-item
      v-for="item in items"
      :key="item"
    >
    <v-img
        :src="item"
    >
    </v-img>
    </v-carousel-item>
  </v-carousel>
</template>

<script>
  export default {
    data: () => ({
      model: 0,
      items: [
        'introduce1.svg',
        'introduce2.svg',
        'introduce3.svg',
        'introduce4.svg',
        'introduce5.svg'
      ],
    }),
  }
</script>
