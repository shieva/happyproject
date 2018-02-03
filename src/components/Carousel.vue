<template>
  <v-carousel hide-controls>
    <v-carousel-item v-for="(item,i) in items" :src="item.src" :key="i"></v-carousel-item>
  </v-carousel>
</template>
<script>
export default {
  props: {
    items: {
      type: Array
    }
  }
}
</script>
