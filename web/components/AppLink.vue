<template>
  <nuxt-link :to="to" :class="{ link: true, 'link--bullet': bullet }">
    <slot></slot>
  </nuxt-link>
</template>

<script>
export default {
  props: {
    to: {
      type: String,
      required: true,
    },
    bullet: {
      type: Boolean,
      default: false,
    },
  },
}
</script>

<style scoped>
a {
  color: darkred;
}
.link--bullet {
  padding-left: theme(spacing.4);
  background-image: url("data:image/svg+xml, %3Csvg%20width%3D'5'%20height%3D'5'%20viewBox%3D'0055'%20fill%3D'none'%20xmlns%3D'http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg'%3E%3Crect%20width%3D'5'%20height%3D'5'%20fill%3D'%23a52626'%2F%3E%3C%2Fsvg%3E");
  background-repeat: no-repeat;
  background-position: left center;
}
</style>
