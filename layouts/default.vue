<template>
  <v-app>
    <v-toolbar
      color="blue darken-3"
      dark
      app
      fixed>
      <v-toolbar-title
        style="width: 300px"
        class="ml-0 pl-3">
        <v-toolbar-side-icon
        @click.stop="drawer = !drawer"/>
        <span class="hidden-sm-and-down">Google</span>
      </v-toolbar-title>
      <v-spacer/>
      <v-btn icon>
        <v-icon>notifications</v-icon>
      </v-btn>
      <v-btn
        icon
        large>
        <v-avatar
          size="32px"
          tile>
          <img src="https://cdn.vuetifyjs.com/images/logos/logo.svg" alt="Vuetify">
        </v-avatar>
      </v-btn>
    </v-toolbar>
    <v-content>
      <v-container>
        <nuxt/>
      </v-container>
    </v-content>
    <v-btn
      color="blue"
      dark
      fab
      fixed
      bottom
      right
      small>
      <v-icon>keyboard_arrow_up</v-icon>
    </v-btn>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      drawer: false
    }
  }
}
</script>
