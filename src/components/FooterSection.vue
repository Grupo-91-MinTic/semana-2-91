<template>
    <footer>
        <div class="container-fluid text-white bg-dark">
            <div class="row p-5 mb-5">
                <div class="col-6">
                    <a class="mx-auto d-block text-center" :href="repository" target="blank">
                        <img :src="icons[0]"/> <br> <strong>Link del repositorio</strong>
                    </a>
                    <hr>
                    <p class="text-center">{{description}}</p>
                </div>
                <div class="col-6 badge">
                    <a :href="icons[1]" target="blank">
                        <img class="text-center" src="https://img.icons8.com/dusk/64/000000/linkedin.png"/>{{names[0]}} {{charges[0]}}
                    </a>
                    <br>
                    <a href="https://github.com/AndresMpa" target="blank">
                        <img class="text-center" :src="icons[0]"/>{{names[0]}} {{charges[0]}}
                    </a>
                    <hr>
                    <a href="https://github.com/carSneider99" target="blank">
                        <img class="text-center" :src="icons[0]"/>{{names[1]}} {{charges[0]}}
                    </a>
                    <hr>
                    <a href="https://github.com/AlejoCM12" target="blank">
                        <img class="text-center" :src="icons[0]"/>{{names[2]}} {{charges[0]}}
                    </a>
                    <hr>
                    <a href="https://github.com/JuanSebOrduz" target="blank">
                        <img class="text-center" :src="icons[0]"/>{{names[3]}} {{charges[0]}}
                    </a>
                </div>
            </div>
        </div>        
    </footer>
</template>
<script>
export default {
    name: "FooterSection",
    data(){
        return{
            icons: ['https://img.icons8.com/dusk/64/000000/github.png', 'https://www.linkedin.com/in/andr%C3%A9s-m-prieto-263a511b7/'],
            repository: 'https://github.com/Grupo-91-MinTic/semana-2-91',
            description: 'Este proyecto se creo para sustentar lo aprendido en el sprint II del ciclo 3, usando Vue, Boostrap, JS',     
            names: ['Andrés Manuel Prieto Álvarez', 'Carlos Sneider Soto Sogamoso', 'Harold Alejandro Caicedo', 'Juan Sebastion Ortiz'],
            charges: ['(Main frontend developer)', '(Main backend developer)', '(Frontend developer)', '(Backend developer)']
        }
    }
}
</script>