<template>
  <v-app>
    <v-app-bar app color="primary" dark>
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
          transition="scale-transition"
          width="40"
        />

        <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
          width="100"
        />
      </div>

      <v-spacer></v-spacer>

      <v-btn
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
        text
      >
        <span class="mr-2">Latest Release</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn>
    </v-app-bar>
    <v-main>
      main
      <hr />
      swipper
      <br />
      <br />
      <br />
      <br />
      <br />
      swipper
      <hr />
      home
      <br />
      <br />
      <br />
      <br />
      <br />
      <br />

      <br />
      <br />
      <br />
      <br />
      <br />
      <br />
      <br />
      <br />

      <br />
      <br />
      <br />
      <br />
      <br />
      <br />
      <br />
      <br />

      <br />
      <br />
      <br />
      <br />
      <br />
      <br />
      <br />

      <router-view />
      main

      <hr />
    </v-main>

    <hr />
    <About />
    <hr />
    <v-bottom-navigation v-model="bottomNav" color="primary" fixed="true">
      <v-btn value="1">
        <span>主页</span>
        <v-icon>mdi-home</v-icon>
      </v-btn>

      <v-btn value="2">
        <span>分享</span>
        <v-icon>mdi-share</v-icon>
      </v-btn>

      <v-btn value="3">
        <span>购物车</span>
        <v-icon>mdi-cart</v-icon>
      </v-btn>

      <v-btn value="4">
        <span>管理</span>
        <v-icon>mdi-cog</v-icon>
      </v-btn>

      <v-btn value="5">
        <span>我的</span>
        <v-icon>mdi-account</v-icon>
      </v-btn>
    </v-bottom-navigation>
  </v-app>
</template>

<script lang="ts">
import Vue from 'vue';
import About from './views/About.vue';
export default Vue.extend({
  name: 'App',
  components: {
    About,
  },
  data: () => ({
    bottomNav: '3',
  }),
});
</script>
