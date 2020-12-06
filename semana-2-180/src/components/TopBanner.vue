<template>
<div>
<header class="header">
        
        <!-- Menú -->
    
    
    
    
    
    
    
    
         <!-- carousel -->
        
     
    
    
    <top-menu></top-menu>

    <div id="carouselExampleCaptions" class="carousel slide" data-ride="carousel">
             <ol class="carousel-indicators">
                 <li data-target="#carouselExampleCaptions" data-slide-to="0"
                class="active"></li>
                 <li data-target="#carouselExampleCaptions" data-slide-to="1" class=""></li>
                 <li data-target="#carouselExampleCaptions" data-slide-to="2" class=""></li>
             </ol>
            <div class="carousel-inner">
                <div class="carousel-item active">
                     <img src="@/assets/i1.jpg" style="width:1555px;height:400px">
                     <!--  -->
                     <div class="carousel-caption d-none d-md-block">
                         <h5>Primera imagen</h5>
                         <p>Representación del cine.</p>
                     </div>
                 </div>
                     <div class="carousel-item">
                         
                         <img src="@/assets/i2.jpg" style="height:400px" >
                         <div class="carousel-caption d-none d-md-block">
                             <h5>Segunda imagen</h5>
                             <p>Representación del cine2.</p>
                         </div>
                     </div>
                     <div class="carousel-item">
                         <img src="@/assets/i3.jpg"  style="width:1555px;height:400px">
                         <div class="carousel-caption d-none d-md-block">
                             <h5>Tercera imagen</h5>
                             <p>Praesent commodo cursus magna, vel scelerisque nisl
                            consectetur.</p>
                         </div>
                     </div>
             </div>
    
             <a class="carousel-control-prev" href="#carouselExampleCaptions" role="button" data-slide="prev">
                 <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                 <span class="sr-only">Previous</span>
             </a>
             <a class="carousel-control-next" href="#carouselExampleCaptions" role="button" data-slide="next">
                 <span class="carousel-control-next-icon" aria-hidden="true"></span>
                 <span class="sr-only">Next</span>
             </a>
         </div>
         </header>
</div>
</template>


<script>
import TopMenu from './TopMenu.vue';
export default {
  components: { 
      TopMenu },
  name: "TopBanner",
};
</script>

<style scoped>
</style>

