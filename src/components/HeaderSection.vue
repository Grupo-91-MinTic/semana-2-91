<template>
<div>
<!-- Image and text -->
 <nav class="navbar navbar-expand-lg sticky-top navbar-dark bg-dark ">
    <div class="collapse navbar-collapse justify-content-end " id="navbarNav ">
        <ul class="navbar-nav ">
            <li class="nav-item active ">
                <a class="nav-link " href="#header ">Menu</a>
            </li>
            <li class="nav-item ">
                <a class="nav-link " href="#services ">Services</a>
            </li>
            <li class="nav-item ">
                <a class="nav-link " href="#news ">News</a>
            </li>
            <li class="nav-item ">
                <a class="nav-link " href="#team ">Team</a>
            </li>
            <li class="nav-item ">
                <a class="nav-link" href="#footer ">Info</a>
            </li>
        </ul>
    </div>
</nav>

<!-- carousel -->
<div id="carouselExampleCaptions header" class="carousel slide" data-ride="carousel">
    <ol class="carousel-indicators bg-dark">
        <li data-target="#carouselExampleCaptions" data-slide-to="0" class="active"></li>
        <li data-target="#carouselExampleCaptions" data-slide-to="1" class=""></li>
        <li data-target="#carouselExampleCaptions" data-slide-to="2" class=""></li>
    </ol>
    <div class="carousel-inner">
        <div class="carousel-item active">
            <img class="bd-placeholder-img bd-placeholder-img-lg d-block w-100" src="https://www.misiontic2022.gov.co/746/articles-151672_foto_marquesina.jpg" alt="Los Tips Mas TIC">
            <div class="carousel-caption d-none d-md-block text-white" style="background: rgba(0,0,0,0.65)">
                <h5>MISION TIC 2020</h5>
                <p>Aprendizaje en línea con MisiónTIC2022.</p>
            </div>
        </div>
        <div class="carousel-item">
            <img class="bd-placeholder-img bd-placeholder-img-lg d-block w-100" src="https://micrositios.mintic.gov.co/plan_5g/img/plan_5g_header.png?v2" alt="Tecnología 5G avanza">
            <div class="carousel-caption d-none d-md-block text-white" style="background: rgba(0,0,0,0.65)">
                <h5>Tecnolgia 5G</h5>
                <p>El Ministerio de las Tecnologías de la Información y las Comunicaciones (MinTIC) avanza en la tecnología 5G.</p>
            </div>
        </div>
        <div class="carousel-item">
            <img class="bd-placeholder-img bd-placeholder-img-lg d-block w-100" src="https://mintic.gov.co/portal/604/articles-160610_foto_marquesina.jpg" alt="Colombia Gana premio">
            <div class="carousel-caption d-none d-md-block text-white" style="background: rgba(0,0,0,0.65)">
                <h5>Colombia Gana</h5>
                <p>El Ministerio TIC ganó premio internacional por su iniciativa Centro de Relevo.</p>
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
</div>
</template>
<script>
export default {
    name: "HeaderSection",
    data(){
        return{
            
        }
    }
}
</script>