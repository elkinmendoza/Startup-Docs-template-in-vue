<template>
  <v-app>
  
    <headerA>

    </headerA>
      <menuDrawerA>

    </menuDrawerA>
    <v-content class="grey lighten-5">

    </v-content>
    <footerA>

    </footerA>
  </v-app>
</template>

<script>
  import headerA from './components/header';
  import menuDrawerA from './components/menudrawer.vue';
  import footerA from './components/footer';

export default {
  name: 'App',

  components: {
      headerA,
      footerA,
      menuDrawerA
    },
  data: () => ({
    //
  }),
};
</script>


<style>

@import url('https://fonts.googleapis.com/css2?family=Montserrat&family=Noto+Sans&family=Oswald&family=Roboto&display=swap');

*{
font-family: 'Roboto', sans-serif;
font-family: 'Montserrat', sans-serif;
font-family: 'Oswald', sans-serif;
font-family: 'Noto Sans', sans-serif;


}
:root {
  --color1: rgba(245, 230, 232, 1);
  --color2: rgba(213, 198, 224, 1);
  --color3:  rgba(170, 161, 200, 1);
  --color4: rgba(150, 122, 161, 1);
  --color5: rgba(25, 42, 81, 1);
}


/* GRADIENT */
$gradient-top: linear-gradient(0deg, #f5e6e8ff, #d5c6e0ff, #aaa1c8ff, #967aa1ff, #192a51ff);
$gradient-right: linear-gradient(90deg, #f5e6e8ff, #d5c6e0ff, #aaa1c8ff, #967aa1ff, #192a51ff);
$gradient-bottom: linear-gradient(180deg, #f5e6e8ff, #d5c6e0ff, #aaa1c8ff, #967aa1ff, #192a51ff);
$gradient-left: linear-gradient(270deg, #f5e6e8ff, #d5c6e0ff, #aaa1c8ff, #967aa1ff, #192a51ff);
$gradient-top-right: linear-gradient(45deg, #f5e6e8ff, #d5c6e0ff, #aaa1c8ff, #967aa1ff, #192a51ff);
$gradient-bottom-right: linear-gradient(135deg, #f5e6e8ff, #d5c6e0ff, #aaa1c8ff, #967aa1ff, #192a51ff);
$gradient-top-left: linear-gradient(225deg, #f5e6e8ff, #d5c6e0ff, #aaa1c8ff, #967aa1ff, #192a51ff);
$gradient-bottom-left: linear-gradient(315deg, #f5e6e8ff, #d5c6e0ff, #aaa1c8ff, #967aa1ff, #192a51ff);
$gradient-radial: radial-gradient(#f5e6e8ff, #d5c6e0ff, #aaa1c8ff, #967aa1ff, #192a51ff);


</style>