<script>
import AppButtonTran from "./AppButtonTran.vue";
import Title from "./Title.vue";
import Contacts from "./Contacts.vue";
import CardFooter from "./CardFooter.vue";

export default {

    data() {
        return {
            firstCard:
            {
                title: "About",
                list: ["The Company", "Insitutonal", "Social & Events", "Innovation", "Environment", "Technology"]
            },

            secondCard:

            {
                title: "Support",
                list: ["Industrialized", "Chemical", "Packaged Liquids", "Construction", "Laminated Wood", "And others"]
            },

            thirdCard:
            {
                title: "Transport",
                list: ["Responsibility", "Terms of Use", "About Cookies", "Privacy policy", "Accessibility", "Information"]
            },




        }
    },
    components: { AppButtonTran, Title, Contacts, CardFooter, }

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
                    <CardFooter :card="firstCard" />
                </div>
                <div class="col">
                    <CardFooter :card="secondCard" />
                </div>
                <div class="col">
                    <CardFooter :card="thirdCard" />
                </div>

            </div>

        </div>

    </section>
</template>


<style scoped lang="scss">
@use "./style/partials/variables" as *;
@use "./style/general.scss";

.wrapper {
    background-color: $Shark;
}

.container {
    padding-top: 5rem;
    padding-bottom: 5rem;
}

p {
    color: $White;
}
</style>