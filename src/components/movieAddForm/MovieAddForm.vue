<template>
  <div class="movieAddForm">
      <h3>Yangi kino qo'shish</h3>
      <form class="add-form d-flex">
          <input type="text" class="form-control new_movie_labale" placeholder="Qanday kino?">
          <input type="text" class="form-control new_movie_labale" placeholder="Necha marotaba ko'rilgan?">
          <button type="submit" class="btn btn-outline-dark">Qo'shish</button>
      </form>
  </div>
</template>

<script>
export default {
    name: "MovieAddForm"
}
</script>

<style scoped>
  .movieAddForm{
      margin-top:2rem ;
      padding: 1.5rem;
      background-color: #fcfaf5;
      border-radius: 4px;
      box-shadow: 15px 15px 15px rgba(0, 0, 0, 0.15);
  }
</style>