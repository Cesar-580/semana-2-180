<template>
         <nav class="navbar navbar-expand-lg sticky-top navbar-dark bg-dark ">
             <a class="navbar-brand " href="# ">
    
             <img src="@/assets/ico.png" width="30 " height="30" 
             class="d-inline-block align-top " alt=" " loading="lazy ">Películas</a>
    
             <div class="collapse navbar-collapse justify-content-end " id="navbarNav ">
                 <ul class="navbar-nav">
                     <li class="nav-item active ">
                         <a class="nav-link " href="# ">Home <span class="sr-only">(current)</span></a>
                     </li>
                     <li class="nav-item">
                         <a class="nav-link " href="# ">Search movies</a>
                     </li>
                     <li class="nav-item">
                         <a class="nav-link " href="# ">Donate</a>
                     </li>
                     <li class="nav-item">
                         <a class="nav-link disabled " href="# " tabindex="-1" ariadisabled="true ">Disabled</a>
                     </li>
                 </ul>
             </div>
         </nav>
</template>


<script>
export default {
  name: "TopMenu",
};
</script>

<style scoped>
</style>

