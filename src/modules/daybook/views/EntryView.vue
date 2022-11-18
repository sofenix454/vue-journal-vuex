<template>
  <div class="entry-title d-flex justify-content-between p-2">
    <div>
        <span class="text-success fs-3 fw-bold">15</span>
        <span class="mx-1 fs-3 ">Diciembre</span>
        <span class="mx-2 fs-4 fw-light">2022, Martes</span>
    </div>

    <div>
        <button class="btn btn-danger mx-2">
            Borrar
            <i class="fa fa-trash-alt"></i>
        </button>

        <button class="btn btn-primary mx-2">
            Subir foto
            <i class="fa fa-upload"></i>
        </button>
    </div>
  </div>
  <hr>
  <div class="d-flex flex-column px-3 h-75">
    <textarea
        placeholder="¿Que sucedio hoy?"
    ></textarea>

  </div>
  <img 
  src="https://images.unsplash.com/photo-1585468274952-66591eb14165?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxleHBsb3JlLWZlZWR8Mnx8fGVufDB8fHx8&w=1000&q=80" 
  alt="img"
  class="img-thumbnail">
  <Fab icon="fa-save"/>
</template>

<script>
import { defineAsyncComponent } from 'vue'
export default {

    components:{
        Fab: defineAsyncComponent(()=> import('../components/Fab.vue'))
    }
}
</script>

<style lang="scss" scoped>
textarea {
    font-size: 20px;
    border: none;
    height: 100%;
    &:focus {
        outline: none;
    }
}
img {
    width: 200px;
    position: fixed;
    bottom: 100px;
    right: 20px;
}
</style>