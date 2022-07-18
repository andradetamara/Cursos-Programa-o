<template>
  <b-container>
    
    <b-row cols="3">
      <CardView v-for="curso in cursos" :key="curso.id" :nome="curso.nome" :imagem="curso.imagem"></CardView>
    
    </b-row>
  </b-container>
</template>

<script>
// @ is an alias to /src
import CardView from '@/components/CardView.vue'

export default {
  name: 'HomeView',
  data() {
    return {
      cursos: []
    }
  },
  components: {
    CardView,
  },
  mounted() {
    this.fetchData();
  },
  methods: {
    //async para gravar
    async fetchData() {
      const res = await fetch("Curso.json");
      const val = await res.json();
      this.cursos = val;
      //console.log(val);
    }
  }
}
</script>
