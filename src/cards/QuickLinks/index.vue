<template>
  <v-card-text id="quick-links">
    <component v-if="settings.links.length" :is="cmp" :data="links" :size="size - 7"/>
    <div v-else class="text-xs-center">
      <v-icon x-large>find_in_page</v-icon>
      <h2 v-t="'QuickLinks.empty'" class="subheading"/>
    </div>
  </v-card-text>
</template>
<script src="./main.js"></script>
<style lang="scss" rel='stylesheet/scss' src="./style.scss" scoped></style>
