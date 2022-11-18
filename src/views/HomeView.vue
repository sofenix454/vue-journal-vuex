<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
  </div>
  <button @click="goToDayBook" class="btn btn-primary" >PRIMARY</button>
  <button class="btn btn-secondary">SECON</button>
</template>
<script>
export default {
  methods: {
    goToDayBook() {
      this.$router.push({name:'no-entry'})
    }
  }
}

</script>