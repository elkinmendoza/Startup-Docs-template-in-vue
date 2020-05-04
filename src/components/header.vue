<template>
    <v-app-bar
      app
      flat
      absolute
      class="white pl-12 pr-12"
      elevate-on-scroll
      scroll-target="#scrolling-techniques-7"
    >



      <v-toolbar-title class="pr-1">Movie</v-toolbar-title>

      <div class="d-flex  grey--text pl-12 hidden-sm-and-down" >

          <a  class="grey--text pa-5 hidden-sm-and-down"  outlined tile href="#">Features</a>
          <a  class="grey--text pa-5 hidden-sm-and-down" outlined tile href="#">Docs</a>
          <a  class="grey--text pa-5 hidden-sm-and-down" outlined tile href="#">Tutorials</a>
          <a  class="grey--text pa-5 hidden-sm-and-down" outlined tile href="#">Team</a>
            

      
      </div>

      <v-spacer></v-spacer>

          <v-btn class="ma-2" outlined color="deep-purple">Get Started</v-btn>
      <v-app-bar-nav-icon class="hidden-md-and-up"></v-app-bar-nav-icon>




    </v-app-bar>

</template>

<script>

export default {
  name: 'headerA',

  components: {
  },

  data: () => ({
    //
  }),
  methods:{

  },
  computed:{

  }
};
</script>
