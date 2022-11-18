<template>
  <div class="entry-container mb-3 pointer p-2" @click="$router.push({name:'entry', params:{id:1}})">
    <div class="entry-title d-flex">
        <span class="text-success fs-5 fw-bold">20</span>
        <span class="mx-1 fs-light">Diciembre</span>
        <span class="mx-2 fs-5">2022</span>
    </div>
    <div class="entry-description">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ducimus blanditiis dicta, consequatur soluta molestiae cumque dolor itaque sint laboriosam earum amet sit velit officia tempore ex provident. Nulla, cupiditate soluta.

    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
.entry-container  {
    border-bottom: 1px solid #2c3e50;
    transition: 0.2s all ease-in;

    &:hover {
        background-color: lighten($color: grey, $amount:40) ;
        transition: 0.2s all ease-in;

    }
    .entry-description {
        font-size: 12px;
    }
}

</style>