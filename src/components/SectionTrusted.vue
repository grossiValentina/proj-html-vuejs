<script>

export default {
    data() {
        return {
            card: [
                {
                    image: "./logo-1.png",
                    content: "Lorem ipsum dolor, sit amet consectetur adipisicing elit. Necessitatibus non maioret"
                },
                {
                    image: "./logo-2.png",
                    content: "Lorem ipsum dolor, sit amet consectetur adipisicing elit. Necessitatibus non maioret"
                },
                {
                    image: "./logo-3.png",
                    content: "Lorem ipsum dolor, sit amet consectetur adipisicing elit. Necessitatibus non maioret"
                },
            ]
        }
    },
}
</script>


<template>
    <section class="wrapper">

        <!--  container risultati  -->
        <div class="my-container">
            <div class="text-center">
                <h5 class="mb-3">CUSTOMER TESTIMONIALS</h5>
                <div class="d-flex title">
                    <h2 class="pe-2">Trusted</h2>
                    <h2 class="title-bg ps-2 pe-2 mb-3">Feedback</h2>
                </div>
                <p class="text-center">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Necessitatibus non maiores
                    eos adipisci vel consectetur cumque, explicabo veritatis rem deserunt </p>
            </div>
        </div>


        <div class="container mt-4">
            
                <!--  card feedback -->
                <div class="d-flex justify-content-between section-card">

                    <div v-for="item in card" class="card" style="width: 19rem;">
                        <div class="card-body">
                            <div class="d-flex justify-content-between">
                                <img :src="`/assets/img` + `item.image`" alt="">
                            </div>
                            <p class="card-text">{{ item.content }}</p>
                            <i class="icon fa-solid fa-quote-right"></i>
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
    padding-top: 5rem ;
    padding-bottom: 5rem;
    width: 100%;
    background-color: $Woodsmoke ;
}

.my-container {
    width: 60%;
    margin: 0 auto;
}

.card {
    background-color: $Shark;
    position: relative;
}
.icon{
    position: absolute;
    bottom: 0;
    right: 0;
    padding: .5rem;
    font-size: 1.5rem;
    color: $MidGray;
}

img {
    filter: grayscale(100%);
    width: 6rem;
}

.title {
    justify-content: center;
    color: $White;
}

h6 {
    color: $White;
}

p {
    color: $White;
}

.title-bg {
    background-color: rgba($FountainBlue, 0.5);
    color: $White;
}
</style>