<template>
  <v-app>
    <v-navigation-drawer app :mini-variant.sync="mini">
      <v-list>
        <v-list-item class="px-2">
          <v-list-item-avatar>
            <v-img src="https://randomuser.me/api/portraits/women/85.jpg"></v-img>
          </v-list-item-avatar>
          <v-list-item-title class="title">Admin</v-list-item-title>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar app>
      <v-app-bar-nav-icon @click="mini = !mini" v-if="mini">
        <v-icon> mdi-format-list-bulleted </v-icon>
      </v-app-bar-nav-icon>
      <v-app-bar-nav-icon @click="mini = !mini" v-else>
        <v-icon> mdi-dots-vertical </v-icon>
      </v-app-bar-nav-icon>
      <v-toolbar-title>Dashboard</v-toolbar-title>
    </v-app-bar>

    <v-main> </v-main>
  </v-app>
</template>

<script>
export default {
  name: "App",

  components: {},

  data: () => ({
    mini: true,
  }),
};
</script>
