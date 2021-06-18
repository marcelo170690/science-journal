<template>
  <v-card flat>
    <v-tabs vertical>
      <v-tab>
        <v-icon left>
          mdi-language-python
        </v-icon>
        Semana 1
      </v-tab>
      <v-tab>
        <v-icon left>
          mdi-lock
        </v-icon>
        Semana 2
      </v-tab>
      <v-tab>
        <v-icon left>
          mdi-access-point
        </v-icon>
        Semana 3
      </v-tab>

      <v-tab-item>
        <Week1/>        
      </v-tab-item>
      <v-tab-item>
        aaaa
      </v-tab-item>
      <v-tab-item>
        ssss
      </v-tab-item>
    </v-tabs>
  </v-card>
</template>

<script>
import Week1 from '@/components/week1/Week1';
export default {
  components: {
    Week1,
  },
}
</script>