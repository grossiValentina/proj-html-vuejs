<script>
import AppButton from "./AppButton.vue";
import AppButtonTran from "./AppButtonTran.vue";
import Title from "./Title.vue";
import Contacts from "./Contacts.vue";

export default {
    data() {
        return {
    
            menu: [
                {
                    title: "HOME"
                },
                {
                    title: "ABOUT"
                },
                {
                    title: "SERVICES"
                },
                {
                    title: "PROCESS"
                },
                {
                    title: "TESTIMONIALS"
                }
            ]
        }
    },
    components: { AppButton, AppButtonTran, Title, Contacts, }

};


</script>


<template>
    <section class="wrapper">

        <div class="container">
            <!-- barra recapiti e orari -->
            <div class="info d-flex justify-content-between pt-2">

                <div class="opening d-flex">
                    <p><i class="fa-solid fa-clock px-1"></i>Open Hours: Mon - Sat - 9:00 - 18:00</p>
                </div>

                <div class="contacts d-flex">
                    <!-- contatti riutilizzabili -->
                    <Contacts class="d-flex mx-4" contact="contact"/>
                    <p class="px-3"><i class="fa-brands fa-facebook"></i></p>
                    <p class="px-3"><i class="fa-brands fa-twitter"></i></p>
                    <p class="px-3"><i class="fa-brands fa-linkedin"></i></p>
                </div>

            </div>
        </div>
    </section>

    <!-- navbar con informazioni -->
    <section class="wrapper-search">
        <div class="container">
            <div class="navbar d-flex justify-content-between">

                 <!-- titolo riutilizzabile  -->
                <div class="pt-4">
                    <Title titleStyle="titleStyle" />
                </div>

                <!-- link ripetuti  -->
                <div class="d-flex">
                    <div class="menu d-flex">
                        <ul v-for="item in menu" :key="item.title">
                            <li><a class="text-decoration-none fw-bold" href="">{{ item.title }}</a></li>
                        </ul>
                    </div>

                    <div class="pt-4">
                        <i class="fa-regular fa-user text-center px-4"></i>
                    </div>
                    <!-- elemento bottone  -->
                    <div class="mt-3">
                        <AppButton buttonText="GET IN TOUCH" />
                    </div>
                </div>
            </div>

            <!-- titolo del main e contenuto  -->
            <div class="my-container">
                <h5>LOGISTICS SERVICE</h5>
                <h1 class="fw-bold">CARGO TRANSPORT</h1>
                <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Soluta quod, reiciendis impedit architecto sunt
                    nulla consequatur, corporis ducimus doloremque hic, eligendi aut quidem totam qui ratione nam explicabo.
                    Est, quaerat.</p>
                <!-- bottoni riutilizzabili  -->
                <div class="d-flex align-items-end pt-2">
                    <AppButton buttonText="GET IN TOUCH" />
                    <AppButtonTran class="ms-3 align-items-end" buttonText="READ MORE" />
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
    height: 40px;
    background-color: $MidGray;

}

.wrapper-search {
    width: 100%;
    background-image: url("../assets/img/bg-9.jpg");
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    height: 100vh;
}

.my-container {
    width: 40%;
    padding-top: 8rem;

    h1 {
        color: $White;
        font-size: 4rem;
    }

    h5 {
        color: $FountainBlue;
    }

    p {
        color: $White;
    }

}

.info {
    color: $White;
    font-size: 13px;
}

ul {
    list-style-type: none;
    padding-top: 1.5rem;
    font-size: 15px;

    a {
        color: $White;
    }
}

h4 {
    color: $White;
}

i {
    color: $White;
}
</style>