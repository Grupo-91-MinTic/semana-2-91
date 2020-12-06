<template>
    <div class="container-fluid">
        <div class="row justify-content-center align-content: flex-start mb-5">
            <div class="col-lg-6 col-xs-12 col-lg-4 mt-4"  v-for="(noticia,index) of news" :key="index">
                <div class="d-flex flex-direction:column justify-content-center ">
                    <div class="card h-100">
                        <div>
                            <h3 align="center">{{noticia.title}}</h3>
                        </div>
                        <div class="d-flex justify-content-center p-2">
                            <img :src="noticia.urlToImage" alt="News-Image" height="280px">
                        </div>
                        <div class="card-body bg-dark">
                            <p class="card-text text-justify text-white">
                                {{noticia.description}}
                            </p>
                            <a :href="noticia.url" >Leer más</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import axios from "axios";
export default {
    name: 'NewsSection',
    data(){
        return{
            news: null
        }
    },
    mounted(){
        let url = "https://newsapi.org/v2/everything?q=Tecnología&languaje=es&pageSize=4&apiKey=20d872061354491e93299e59b4fc029c";
        axios.get(url)
        .then((result) => {
            this.news = result.data.articles
            //console.log(this.news)
        })
    }
    
}
</script>

<style scoped>

</style>