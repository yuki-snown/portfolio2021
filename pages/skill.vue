<template>
  <v-treeview
    open-all
    hoverable
    :items="items"
    class="text-h5 mb-2 white--text"
  ></v-treeview>
</template>

<script>
  export default {
    data: () => ({
      items: [
        {
          id: 1,
          name: 'Python (4年)',
          children: [
            { id: 2, name: 'Flask'},
            { id: 3, name: 'Django' },
            { id: 4, name: 'Keras' },
            { id: 5, name: 'Pytorch' },
          ],
        },
        {
          id: 10,
          name: 'Ruby (2年)',
          children: [
            { id: 11, name: 'Ruby on Rails' },
          ],
        },
        {
          id: 6,
          name: 'Javascript (1年)',
          children: [
            { id: 7, name: 'Node.js' },
            { id: 8, name: 'Vue.js' },
            { id: 9, name: 'Nuxt.js' },
          ],
        },
        {
          id: 12,
          name: 'Dart (1年)',
          children: [
            { id: 13, name: 'Flutter' },
          ],
        },
        {
          id: 15,
          name: 'C# (2年)',
          children: [
            { id: 16, name: '.NET' },
          ],
        },
        {
          id: 17,
          name: 'Docker (3年)',
          children: [
            { id: 18, name: 'BuildKit' },
            { id: 19, name: 'compose' },
          ],
        },
        {
          id: 20,
          name: 'AWS (3年)',
          children: [
            { id: 21, name: 'EC2' },
            { id: 22, name: 'Light Sail' },
            { id: 23, name: 'ALB' },
            { id: 24, name: 'lambda' },
            { id: 25, name: 'API gateway' },
          ],
        },
      ],
    }),
  }
</script>
