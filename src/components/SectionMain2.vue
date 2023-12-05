<script>

import AppButtonTran from './AppButtonTran.vue';

export default {
    data(){
        return{
            card: [
                {
                    icon: "fa-truck-ramp-box",
                    title: "Technology",
                    content: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Odit natus autem omnis"
                },
                {
                    icon: "fa-temperature-low",
                    title: "Reefer Carco",
                    content: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Odit natus autem omnis" 
                },
                {
                    icon: "fa-truck",
                    title: "Dry Carco",
                    content: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Odit natus autem omnis" 
                },
            ]

        }
    },

    components: { AppButtonTran }
}
</script>


<template>
    <section class="wrapper">
        <div class="container">

            <h5 class="pb-3">ROAD TRANSPORT</h5>
            <div class="d-flex">
                <h2 class="pe-2">Main</h2>
                <h2 class="title-bg px-2">Services</h2>
            </div>

            <div class="row">

                <!-- colonna paragrafo  -->
                <div class="col-8">
                    <div>
                        <p class="pt-3">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Odit natus autem omnis
                            animi libero quo soluta dolores recusandae nihil ipsum, provident, consectetur obcaecati
                            blanditiis ab sint </p>
                    </div>
                </div>

                <!-- colonna bottone riutilizzabile  -->
                <div class="col-4 pt-3">
                    <AppButtonTran buttonText="SEE ALL" />
                </div>

            </div>

            <!-- cards main services  -->
            <div class="d-flex justify-content-between section-card">

                <div v-for="item in card" class="card" style="width: 19rem;">
                    <div class="card-body">
                        <div class="d-flex justify-content-between">
                            <i :class="item.icon + ' fa-solid'" class="icon"></i>
                            <a href=""><i class="arrow fa-solid fa-arrow-right"></i></a>
                        </div>
                        
                        <h6 class="card-title pt-3 fw-bold">{{ item.title }}</h6>
                        <p class="card-text">{{ item.content }}</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>


<style scoped lang="scss">
@use "./style/partials/variables" as *;
@use "./style/general.scss";

.wrapper {
    width: 100%;
    background-color: $Woodsmoke;
    padding-top: 6rem;
}

h2 {
    color: $White;
}

;

.title-bg {
    background-color: rgba($FountainBlue, 0.5);
    color: $White;
}

;

p {
    color: $White;
};

.section-card{
    padding-bottom: 5rem;
}

.card{
    background-color: $Shark;
    
    h6{
        color: $White;
    };
    .icon{
        color: $FountainBlue;
        background-color: rgba($FountainBlue, 0.3);
        padding: .6rem;
        border-radius: 50%;    
    };
    .arrow{
       color: $FountainBlue;
    }
}
</style>a