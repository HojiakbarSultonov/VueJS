<template>
<ul  class="movie_list list-group">
<MovieListItem v-for="movie in movies" :movie="movie"/>
</ul>
</template>

<script>
import MovieListItem from "@/components/movieListItem/MovieListItem.vue";

export default {
    name: "MovieList",
      components: {MovieListItem},
props:{
        movies:{
            type:Array,
            required:true
        }
}
}
</script>

<style scoped>
.movie_list{
      margin-top:1rem ;
      padding: 1.5rem;
      background-color: #fcfaf5;
      border-radius: 4px;
      box-shadow: 15px 15px 15px rgba(0, 0, 0, 0.15);
}
</style>