<template>
    <article id="team">
        <div class="card badge-info container-fluid mt-5 pt-5" style="width: 18rem;">
            <img :src="member.image​" class="card-img-top" :alt="member.​nombre​">
            <div class="card-body text-center">
                <h3 class="card-title">{{member.​nombre​}}</h3>
                <h6 class="card-text">{{member.rol}}</h6>
                <hr>
                <p class="text-justify">
                    {{member.description}}
                </p>
            </div>
        </div>
    </article>
</template>

<script>
    export default {
        name: "TeamCard",
        props: {
            'member': Object
        }
    }
</script>