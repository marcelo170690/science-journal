<template>
  <v-card
    class="mx-auto"
    :color="color"
    dark
  >
    <v-card-title>
      <span class="text-h6">{{ title }}</span>
    </v-card-title>

    <v-card-text class="text-h6">
      {{ description }}
    </v-card-text>
    <v-divider/>
  </v-card>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: () => {},
    },
    description: {
      type: String,
      default: () => {},
    },
    color: {
      type: String,
      default: () => {},
    },
  }
}
</script>