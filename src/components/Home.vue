<template>
  <v-container class="fill-height">
    <v-responsive class="align-center text-center fill-height">
      <h1>This will be my new Home Page</h1>
      <v-btn @click="IpsumContainer = true">Button</v-btn>
      <v-btn @click="dialog = true">Open Dialog</v-btn>
  
      <v-dialog v-model="dialog" width="auto">
        <!-- Using v-card component for headings, content, etc https://vuetifyjs.com/en/components/cards/ -->
        <v-card class="align-center">
          <v-card-text>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
          </v-card-text>
          <v-card-actions>
            <v-btn @click="dialog = false">Close Dialog centered?</v-btn>
          </v-card-actions>
        </v-card>
      </v-dialog>

      <v-dialog v-model="IpsumContainer" width="auto">
        <v-card class="align-center">
          <v-card-text>
            This is my second Dialog on the same page
          </v-card-text>
          <v-card-actions>
            <v-btn @click="IpsumContainer = false">Close</v-btn>
          </v-card-actions>
        </v-card>
      </v-dialog>      
  
    </v-responsive>
  </v-container>

</template>

<script>
  // "dialog" is the name of the model which is used to generate the dialogs. It's just a variable so doesn't have to have the name "dialog"
  export default {
    data() {
      return {
        dialog: false,  /* Instantiate an empty container for the dialog model */
        IpsumContainer: false,
      }
    },
  }
</script>