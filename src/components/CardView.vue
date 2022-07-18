<template>
    <b-col>
      <b-card 
      :title="nome" 
      style="max-width: 20rem;"  
      tag="article" 
      class="mb-2"
      border-variant="danger"
      header="Curso"
      header-bg-variant="grey"
      header-text-variant="black"
      align="center"
      :img-src= "imagem" 
      img-alt="Image" 
      img-top>
        <b-card-text>
          Just add your desired image size (width & height) after our URL, and you'll get a random image.
        </b-card-text>
        <b-button variant="outline-danger">Sobre</b-button><br/><br/>
        
        <b-button variant="outline-danger">Comprar</b-button>

      </b-card>
    </b-col>
</template>

<script>
export default {
  props:{
    nome: {
      type: String,
      required: true,
    },
    imagem: {
      type:String,
      require: true,
    },
    about: {
    type: String,
    require: true,
    }
  },
}
</script>

<style>
img {
  padding: 1rem;
  width: 20%;
  height: 250px;
  }
</style>

