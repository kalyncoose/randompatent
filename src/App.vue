<template>
  <v-app>
    <v-main>
      <div class="text-center" style="">
        <v-btn :color="colors[getRandomInt(17)]" 
                style="height:100vh;width:100vw;display:block;padding-top:40vh;"
                :href="base_url+getRandomInt(11375651)" tile>
          <span style="font-size:xx-large;font-weight:bolder;">Random Patent</span>
        </v-btn>
      </div>
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',
  components: {

  },
  data: () => ({
    base_url: 'https://patents.google.com/patent/US',
    colors: [
      '#1abc9c',
      '#16a085',
      '#2ecc71',
      '#27ae60',
      '#3498db',
      '#2980b9',
      '#9b59b6',
      '#8e44ad',
      '#f1c40f',
      '#f39c12',
      '#e67e22',
      '#d35400',
      '#e74c3c',
      '#c0392b',
      '#ecf0f1',
      '#bdc3c7',
      '#95a5a6',
      '#7f8c8d'
    ]
  }),
  methods: {
    getRandomInt: function (max) {
      return Math.floor(Math.random() * max);
    }
  },
};
</script>
