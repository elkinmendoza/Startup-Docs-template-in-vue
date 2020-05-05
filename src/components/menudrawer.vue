<template>
   
<v-navigation-drawer
      v-model="drawer"
      absolute
      temporary
      right
      width="80%"
    >
      
  <v-container>
    <v-row>
    <v-row class="pt-4 pl-12 pr-12 text-left" :alignment="space-around">
    <v-col class="col">
      LOGO
    </v-col>
    <v-col class="col text-right">
      X
    </v-col>
    </v-row>
    
    <v-col class="col-12 pa-11">
      <v-list>
        <v-list-group
          v-for="item in items"
          :key="item.title"
          v-model="item.active"
          no-action
        >
          <template v-slot:activator>
            <v-list-item-content>
              <v-list-item-title v-text="item.title"></v-list-item-title>
            </v-list-item-content>
          </template>
  
          <v-list-item
            v-for="subItem in item.items"
            :key="subItem.title"
            
          >
            <v-list-item-content>
              <v-list-item-title v-text="subItem.title"></v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list-group>
      </v-list>
    </v-col>

    </v-row>

  </v-container>
     
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
        {
          action: 'local_activity',
          title: 'Attractions',
          items: [
            { title: 'List Item' },
          ],
        },
        {
          action: 'restaurant',
          title: 'Dining',
          active: true,
          items: [
            { title: 'Breakfast & brunch' },
            { title: 'New American' },
            { title: 'Sushi' },
          ],
        },
        {
          action: 'school',
          title: 'Education',
          items: [
            { title: 'List Item' },
          ],
        },
        {
          action: 'directions_run',
          title: 'Family',
          items: [
            { title: 'List Item' },
          ],
        },
        {
          action: 'healing',
          title: 'Health',
          items: [
            { title: 'List Item' },
          ],
        },
        {
          action: 'content_cut',
          title: 'Office',
          items: [
            { title: 'List Item' },
          ],
        },
        {
          action: 'local_offer',
          title: 'Promotions',
          items: [
            { title: 'List Item' },
          ],
        },
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
