<template>
<div class="app">
   <div class="content">
       <AppInfo/>
       <div class="search-panel">
        <SearchPanel/>
           <AppFilter/>
       </div>
       <MovieList/>
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