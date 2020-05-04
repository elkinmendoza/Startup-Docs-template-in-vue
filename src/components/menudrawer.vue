<template>
   
<v-navigation-drawer
      v-model="drawer"
      absolute
      temporary
      right
      width="80%"
    >
      

      <v-divider></v-divider>

     
    </v-navigation-drawer>



</template>

<script>
import { EventBus } from '../main';

export default {
  name: 'menuDrawerA',

  components: {
  },
  data: () => ({
    drawer:null,
        items: [
          { title: 'Home', icon: 'dashboard' },
          { title: 'About', icon: 'question_answer' },
        ],
    //
  }),
  methods:{

  },
  created (){


        

    EventBus.$on('turnDrawer', () => {
            this.drawer = !this.drawer
    })
  },
};
</script>
