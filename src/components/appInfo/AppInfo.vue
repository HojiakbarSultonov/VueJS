<template>
<div class="appInfo">
    <p class="fs-3 text-uppercase">Barcha kinolar soni: {{AllMoviesCount}}</p>
    <p class="fs-4 text-uppercase">Ko'rilgan kinolar soni: {{favouriteMoviesCount}}</p>
</div>
</template>

<script>
export default {
    props:{
        AllMoviesCount:
            {
                type:Number,
                required:true
            },
        favouriteMoviesCount:
            {
                type:Number,
                required:true
            },
    }
}
</script>

<style scoped>
  .appInfo{
      padding: 1.5rem;
      border-radius: 4px;
    background-color: #fcfaf5;
      box-shadow: 15px 15px 15px rgba(0, 0, 0, 0.15);
  }
</style>