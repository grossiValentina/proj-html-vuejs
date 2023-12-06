<script>
import AppButtonTran from "./AppButtonTran.vue";
import Title from "./Title.vue";
import Contacts from "./Contacts.vue";
import CardFooter from "./CardFooter.vue";

export default {
    data() {
        return {
        Title: [
                {
                    content: "About"
                },
                {
                    content: "Support"
                },
                {
                    content: "Transport"
                },
               
            ]


        }
    },
    components: { AppButtonTran, Title, Contacts, CardFooter }

}
</script>

<template>
    <section class="wrapper">
        <div class="container">
            <div class="row row-cols-4">
                <div class="col">

                    <!-- titolo riutilizzabile  -->
                    <Title titleStyle="titleStyle" />

                    <p>Lorem ipsum dolor sit amet consectetur</p>

                    <!-- contatti riutilizzabili  -->
                    <div class="mt-4 mb-4">
                        <Contacts contact="contact" />
                        <p><i class="p-1 fa-solid fa-location-dot"></i>Main Avenue,987</p>
                    </div>

                    <!-- bottone riutilizzabile  -->
                    <AppButtonTran buttonText="GET IN TOUCH" />
                </div>

                <!-- card con lista riutilizzabili  -->
                <div class="col">
                    <CardFooter />

                </div>



                <div class="col">
                 
                </div>

                <div class="col">
                    
                </div>


            </div>

        </div>

    </section>
</template>


<style scoped lang="scss">
@use "./style/partials/variables" as *;
@use "./style/general.scss";

.wrapper {
    background-color: pink;
}

.container {
    padding-top: 5rem;
    padding-bottom: 5rem;
}

p {
    color: $White;
}

</style>