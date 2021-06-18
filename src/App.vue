<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
    >
      <div class="d-flex align-center">
        <v-icon large>mdi-chart-line</v-icon>
        MARCELO CHOQUE PACHECO - SCIENCE JOURNAL
      </div>
    </v-app-bar>

    <Navbar/>
    <v-main>
      <Container/>
    </v-main>
  </v-app>
</template>

<script>
import Navbar from '@/components/Navbar';
import Container from '@/components/Container';

export default {
  name: 'App',

  components: {
    Navbar,
    Container,
  },

  data: () => ({
    //
  }),
};
</script>
