<template>
  <v-container>
    <v-row>
      <v-col cols="12" md="6">
        <Course
          color="#F7D045"
          title="Curso Básico de Python"
          teacher="Facundo García Martoni"
        />
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="12" md="6"
        v-for="(commet, index) in comments"
        :key="index"
      >
        <CommentCard
          :color="commet.color"
          :title="commet.title"
          :description="commet.description"
          :teacher="commet.teacher"
        />
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import CommentCard from './CommentCard';
import Course from '@/components/Course';
export default {
  components: {
    CommentCard,
    Course,
  },
  data() {
    return {
      comments: [
        {
          color: '#3771A1',
          title: '¿Qué aprendi?',
          description: 'Basicamente aprendí el lenguaje python, la estructura que se maneja en python, ciclos, diccionarios, arrays, etc',
        },
        {
          color: '#3771A1',
          title: '¿Retos?',
          description: 'El cambio que se tiene de javascript a python de da mas en la estructura, y mas aún en los estandares, de comillas simples a dobles, de camel case a snake case, ya sin corchetes etc.',
        },
        {
          color: '#3771A1',
          title: '¿Qué dedo profundizar?',
          description: 'Debo profundizar las funciones propias del lenguaje',
        },
        {
          color: '#3771A1',
          title: '¿Esta semana mejore mi habilidad en ...?',
          description: 'Mas alla del lenguaje python, practique mis habilidades lambda',
        },
      ],
    };
  },
}
</script>