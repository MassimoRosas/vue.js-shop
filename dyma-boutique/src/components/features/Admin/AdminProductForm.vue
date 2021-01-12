<template>
  <form class="d-flex flex-column">
    <h4>Ajouter un produit :</h4>
    <hr class="w-100">
    <div class="form-group p-2">
      <label>Image</label>
      <input type="text" class="form-control" />
    </div>
    <div class="form-group p-2">
      <label>Titre</label>
      <input type="text" class="form-control" />
    </div>
    <div class="form-group p-2">
      <label>Description</label>
      <textarea class="form-control"></textarea>
    </div>
    <div class="form-group p-2">
      <label>Prix</label>
      <input type="number" class="form-control" />
    </div>
    <button class="btn btn-primary m-2">Ajouter</button>
  </form>
</template>

<script>
export default {
  
}
</script>

<style scoped>

</style>