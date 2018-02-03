<template>
  <v-footer height="auto" class="main-footer">
    <v-card
      flat
      tile
      class="indigo lighten-1 white--text text-xs-center footer-card"
    >
      <v-card-text class="secondary">
        <v-btn
          v-for="icon in icons"
          :key="icon"
          icon
          class="mx-3 white--text"
        >
          <v-icon size="24px">{{ icon }}</v-icon>
        </v-btn>
      </v-card-text>
    </v-card>
  </v-footer>
</template>
<script>
export default {
  data: () => ({
    icons: ['fa-facebook', 'fa-twitter', 'fa-google-plus', 'fa-linkedin', 'fa-instagram']
  })
}
</script>
<style>
  .footer>:last-child {
    margin-right: 0px;
  }
  .footer>:first-child {
    margin-left: 0px;
  }
  .main-footer{
    bottom: 0;
    position: fixed;
    width: 100%;
  }
  .footer-card {
    width:100%;
    background-color: #F7AF52 !important;
  }
</style>
