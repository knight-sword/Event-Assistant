<template>
  <div>
    <v-row class="flex-child">
      <v-col class="d-flex justify-center align-center bg-primary-lighten-5" cols="12" md="6">
        <div class="text-center">
          <v-avatar color="grey" size="150" rounded="0">
            <v-img cover src="https://cdn.vuetifyjs.com/images/profiles/marcus.jpg"></v-img>
          </v-avatar>
        </div>
      </v-col>
      <v-col class="d-flex justify-center align-center" cols="12" md="6">456</v-col>
    </v-row>
  </div>
</template>
<style>
.text-center {
  text-align: center;
}
.bg-primary-lighten-5 {
  --v-theme-overlay-multiplier: var(--v-theme-primary-lighten-5-overlay-multiplier);
  background: #d7edff !important;
  color: rgb(var(--v-theme-on-primary-lighten-5)) !important;
}
</style>
