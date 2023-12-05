<script>
import { store } from "../store";
export default {
    data() {
        return {
            card: [
                {
                    number: "01",
                    title: "Collection of information",
                    content: " lorem imsum dolor sit amet consecetur"
                },
                {
                    number: "02",
                    title: "Service Invoice Sending",
                    content: " lorem imsum dolor sit amet consecetur"
                },
                {
                    number: "03",
                    title: "Withdrawal of Cargo",
                    content: " lorem imsum dolor sit amet consecetur"
                },
                {
                    number: "04",
                    title: "Transport Customer Order",
                    content: " lorem imsum dolor sit amet consecetur"
                },
                {
                    number: "05",
                    title: "Successful Delivery",
                    content: " lorem imsum dolor sit amet consecetur"
                },

            ]

        }
    },


}
</script>


<template>
    <section class="wrapper">

        <!--  container procedura logistica  -->
        <div class="my-container">
            <div class="text-center">
                <h5 class="mb-3">HOW IT WORKS IN PRACTICE</h5>
                <div class="d-flex title">
                    <h2 class="title-bg ps-2 pe-2 mb-3">Logistical</h2>
                    <h2 class="ps-2">Procedure</h2>
                </div>
                <p class="text-center">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Necessitatibus non maiores
                    eos adipisci vel consectetur cumque, explicabo veritatis rem deserunt </p>
            </div>
        </div>


        <div class="container-procedure mt-4">
            <div class="row row-cols-5 justify-content-evenly">

                <!--  card punti focali procedura logistica  -->
                <div v-for="item in card" class="col text-center">
                    <div class="number fw-bold mb-3">{{ item.number }}</div>
                    <h6 class="fw-bold">{{ item.title }}</h6>
                    <p>{{ item.content }}</p>
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
}

.my-container {
    width: 60%;
    margin: 0 auto;
}

.container-procedure {
    width: 85%;
    margin: 0 auto;
    margin-bottom: 6rem;
}

.number {
    color: $FountainBlue;
    //background-color: rgba($FountainBlue, 0.5);

}

.title {
    justify-content: center;
}

.title-bg {
    background-color: rgba($FountainBlue, 0.5);
    color: $BlueLagoon;
}
</style>