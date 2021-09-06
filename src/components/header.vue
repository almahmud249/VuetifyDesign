<template>
<div>
    <v-app-bar style="padding: 0px 90px" color="white" flat elevation="6" elevate-on-scroll light fixed>
        <v-toolbar-title class="toolbar_title"> Vuetify app </v-toolbar-title>
        <v-spacer></v-spacer>
        <v-list class="d-flex align-center">
            <v-list-item link v-for="menu in menus" :key="menu.title">
                <v-list-item-title > {{ menu.title }} </v-list-item-title>
            </v-list-item>
        </v-list>
        <v-btn text>
          <v-icon>mdi-magnify</v-icon>
        </v-btn>

   <v-btn outlined color="success">Get Started</v-btn>       
    </v-app-bar>
</div>
</template>

<script>
export default {
  data(){
    return {
      menus:[
        {title:'Home'},
        {title:'Portfolio'},
        {title:'Gallery'},
        {title:'Project'},
        {title:'Contact'},
      ]
    }
  }
};
</script>

<style>
.v-toolbar__title.toolbar_title {
    font-size: 30px;
    color: rgb(70, 155, 70);
    font-family: cursive;
    font-weight: 700;
}
</style>