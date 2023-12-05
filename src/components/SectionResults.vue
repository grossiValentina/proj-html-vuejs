<script>

export default {
    data() {
        return {
            card: [
                {
                    number: "128",
                    title: "Certifications",
                },
                {
                    number: "230",
                    title: "Employees",
                },
                {
                    number: "517",
                    title: "Customers",
                },
                {
                    number: "94",
                    title: "Countries Served",
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
                <h5 class="mb-3">WHAT ARE WE DOING</h5>
                <div class="d-flex title">
                    <h2 class="title-bg ps-2 pe-2 mb-3">Results</h2>
                    <h2 class="ps-2">in Numbers</h2>
                </div>
            </div>
        </div>


        <div class="container-numbers mt-4">
            <div class="row row-cols-5 justify-content-evenly">

                <!--  card punti focali procedura logistica  -->
                <div v-for="item in card" class="col text-center">
                    <div class="number fw-bold mb-3">{{ item.number }}</div>
                    <h6 class="fw-bold">{{ item.title }}</h6>
                </div>

            </div>

        </div>
    </section>
</template>


<style scoped lang="scss">
@use "./style/partials/variables" as *;
@use "./style/general.scss";

.wrapper {
    padding-top: 5rem;
    width: 100%;
    background-image: url("../assets/img/bg-10.jpg");
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    height: 75vh;
}

.my-container {
    width: 60%;
    margin: 0 auto;
}

.container-numbers {
    width: 70%;
    margin: 0 auto;
    margin-bottom: 6rem;
}

.number {
    color: $FountainBlue;
    font-size: 1.5rem;

}

.title {
    justify-content: center;
    color: $White;
}
h6{
    color: $White;
}

.title-bg {
    background-color: rgba($FountainBlue, 0.5);
    color: $White;
}
</style>