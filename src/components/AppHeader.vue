<script>

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

};



</script>


<template>
    <section class="wrapper">

        <div class="container">
            <!-- barra recapiti e orari -->
            <div class="info d-flex justify-content-around pt-2">

                <div class="opening d-flex">
                    <p><i class="fa-solid fa-clock px-1"></i>Open Hours: Mon - Sat - 9:00 - 18:00</p>
                </div>

                <div class="contacts d-flex">
                    <p><i class="fa-solid fa-phone mb-0 px-1"></i>+1(305)1234-5678</p>
                    <p class="px-4"><i class="fa-solid fa-envelope px-1"></i>hello@example.com</p>
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
            <div class="navbar d-flex justify-content-around">

                <div class="d-flex">
                    <h4 class="next ps-3">NEX</h4>
                    <h4>GEN</h4>
                </div>

                <div class="d-flex">
                    <div class="menu d-flex">
                        <ul v-for="item in menu" :key="item.title">
                            <li><a class="text-decoration-none fw-bold" href="">{{ item.title }}</a></li>
                        </ul>
                    </div>

                    <div>
                        <i class="fa-regular fa-user text-center"></i>
                    </div>

                    <div>
                        <button></button>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>


<style scoped lang="scss">
@use "./style/partials/variables" as *;

.wrapper {
    width: 100%;
    height: 40px;
    background-color: $MidGray;

};

.wrapper-search {
    width: 100%;
    background-image: url("../assets/img/bg-9.jpg");
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    height: 100vh;
}

.info {
    color: $White;
    font-size: 13px;
};

ul {
    list-style-type: none;
    padding-top: 1.5rem;

    a {
        color: $White;
    };
};
h4{
    color: $White;
};
.next{
    background-color: $FountainBlue;
    border-top-left-radius: 15px;
    border-bottom-left-radius: 15px; 
}
</style>