<template>

    <v-footer fluid  class="pa-0 transparent">
    
     <v-container b fluid class="pa-12 main-footer caption" >
      <v-row >
     
        <v-col class="col-lg-6 col-md-6 col-sm-12 col-xs-12">
        <h3 class="font-italic font-weight-light">Handcrafted by </h3>
        </v-col>
        <v-col class="col-lg-2 col-md-2 col-sm-6  col-xs-4"  ><h4 class="font-italic font-weight-light">Documentation</h4>
          <a class="grey--text" href="#"> Link 1</a><v-spacer></v-spacer>
          <a class="grey--text" href="#"> Link 1</a><v-spacer></v-spacer>
          <a class="grey--text" href="#"> Link 1</a><v-spacer></v-spacer>
          <a class="grey--text" href="#"> Link 1</a><v-spacer></v-spacer>
       
        </v-col>
        <v-col class="col-lg-2 col-md-2 col-sm-6 col-xs-4"><h4 class="font-italic font-weight-light">Features</h4>
        
          <a class="grey--text" href="#"> Link 1</a><v-spacer></v-spacer>
          <a class="grey--text" href="#"> Link 1</a><v-spacer></v-spacer>
            <a class="grey--text" href="#"> Link 1</a><v-spacer></v-spacer>
       
         </v-col>
        <v-col class="col-lg-2 col-md-2 col-sm-6 col-xs-4"><h4 class="font-italic font-weight-light">Support</h4>
          <a class="grey--text" href="#"> Link 1</a><v-spacer></v-spacer>
          <a class="grey--text" href="#"> Link 1</a><v-spacer></v-spacer>
        </v-col>
        

      </v-row>
      </v-container>
      <v-container fluid class="deep-purple lighten-5 pa-6">
      <v-row >


          <v-col
           >
           <p class="ma-0 blue-grey--text text--lighten-1 overline">
            Fugiat ea nulla ad reprehenderit.
           </p>
          </v-col>
           <v-col
          >
            <p class="ma-0 blue-grey--text text--lighten-1 subtitle text-right overline">
            Fugiat ea nulla ad reprehenderit.
           </p>
          </v-col>
      </v-row>
      </v-container>
      <v-container  dense  fluid class="deep-purple lighten-4 pa-2 overline">
      <v-row   :align="alignment"
          :justify="justify">
      <div>&copy; {{ new Date().getFullYear() }}</div>
      
      </v-row>
      </v-container>
    </v-footer>
</template>

<script>

export default {
  name: 'footerA',

  components: {
  },

  data: () => ({
    alignmentsAvailable: [
          'start',
          'center',
          'end',
          'baseline',
          'stretch',
        ],
        alignment: 'stretch',
        dense: false,
        justifyAvailable: [
          'start',
          'center',
          'end',
          'space-around',
          'space-between',
        ],
        justify: 'center',
  }),
  methods:{

  },
  computed:{

  }
};
</script>
<style>


</style>
