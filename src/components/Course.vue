<template>
  <v-card
    class="mx-auto"
    :color="color"
    dark
  >
    <v-card-title>
      <span class="text-h6">{{ title }}</span>
    </v-card-title>
    <v-divider/>
    <v-card-actions>
      <v-list-item class="grow">
        <v-list-item-avatar color="grey darken-3">
          <v-img
            class="elevation-6"
            alt=""
            src="https://avataaars.io/?avatarStyle=Transparent&topType=ShortHairShortCurly&accessoriesType=Prescription02&hairColor=Black&facialHairType=Blank&clotheType=Hoodie&clotheColor=White&eyeType=Default&eyebrowType=DefaultNatural&mouthType=Default&skinColor=Light"
          ></v-img>
        </v-list-item-avatar>

        <v-list-item-content>
          <v-list-item-title>{{ teacher }}</v-list-item-title>
        </v-list-item-content>
      </v-list-item>
    </v-card-actions>
  </v-card>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: () => {},
    },
    teacher: {
      type: String,
      default: () => {},
    },
    color: {
      type: String,
      default: () => {},
    },
  },
}
</script>