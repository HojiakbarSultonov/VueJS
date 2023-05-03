<template>
<div class="app font-monospace">
   <div class="content">
       <AppInfo :AllMoviesCount="movies.length" :favouriteMoviesCount = 'movies.filter(c=>c.favourite).length
'/>
       <div class="search-panel">
        <SearchPanel/>
           <AppFilter/>
       </div>
       <MovieList :movies="movies"/>
       <MovieAddForm/>
   </div>
</div>

</template>

<script>

import AppInfo from "@/components/appInfo/AppInfo.vue";
import SearchPanel from "@/components/searchPanel/SearchPanel.vue";
import AppFilter from "@/components/appFilter/AppFilter.vue";
import MovieList from "@/components/movieList/MovieList.vue";
import MovieAddForm from "@/components/movieAddForm/MovieAddForm.vue";

export  default {
    components:{
        MovieAddForm,
        MovieList,
        AppFilter,
        SearchPanel,
        AppInfo
    },
    data(){
        return{
            movies:[
                {
                    name:'Jurassic Park',
                    viewers:811,
                    favourite:false,
                    like:true
                },    {
                    name:'Jurassic Park 2',
                    viewers:900,
                    favourite:false,
                    like:false
                },    {
                    name:'Jurassic Park 3',
                    viewers:1011,
                    favourite:true,
                    like:false
                },
            ]
        }
    }
}

</script>

<style>
.app{
    height: 100vh;
    color: black;
}
.content{
    width: 1000px;
    min-height: 700px;
    background-color: #fff;
    margin: 0 auto;
    padding: 5rem 0;
}
.search-panel{
    margin-top: 2rem;
    padding: 1.5rem;
    background-color: #fcfaf5;
    border-radius: 4px;
    box-shadow: 15px 15px 15px rgba(0, 0, 0, 0.15);
}
</style>