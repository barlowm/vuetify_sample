<template>
  <!-- https://codingbeautydev.com/blog/vuetify-app-bar/ -->
  <!-- Documentation was off on the background image. require doesn't work -->
  <!-- image customization is done via the v-slot:image -->
        <v-app-bar
      app
      color="primary"
      dark
      prominent
      image="@/assets/enterprise-1.jpg"
    >
      <template v-slot:image>
        <v-img
          gradient="to top right, rgba(19,84,122,.8), rgba(128,208,199,.8)"
        ></v-img>
      </template>

      <v-app-bar-nav-icon> </v-app-bar-nav-icon>
      <v-toolbar-title>
        <v-icon icon="mdi-circle-slice-6" />
        Essentials Preset
      </v-toolbar-title>

      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>
      
    </v-app-bar>
</template>

<script setup>
  //
</script>
