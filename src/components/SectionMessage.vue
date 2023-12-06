<script>
import AppButton from "./AppButton.vue";
import AppButtonTran from "./AppButtonTran.vue";

export default {
    data() {
        return {


        }
    },
    components: { AppButton, AppButtonTran }
}

</script>

<template>
    <section class="container">
        <div class="row">

            <!-- colonna Get in Touch  -->
            <div class="col-8 me-4">
                <h5>SEND A MESSAGE</h5>

                <div class="d-flex">
                    <h2 class="pe-3">Get in</h2>
                    <h2 class="title-bg ps-2 pe-2">Touch</h2>
                </div>
                <p class="pt-3">Lorem ipsum dolor sit amet consectetur Lorem ipsum dolor</p>

                <!-- gruppi di input  -->
                <div class="row">

                    <div class="col">
                        <div class="form-floating">
                            <input type="text" class="form-control" placeholder="Name" />
                            <label for="floatingInputGrid">Name</label>
                        </div>
                    </div>

                    <div class="col">
                        <div class="form-floating">
                            <input type="text" class="form-control" placeholder="Email" />
                            <label for="floatingInputGrid">Email</label>
                        </div>
                    </div>

                </div>

                <div class="row mt-4">

                    <div class="col">
                        <div class="form-floating">
                            <input type="text" class="form-control" placeholder="Phone" />
                            <label for="floatingInputGrid">Phone</label>
                        </div>
                    </div>

                    <div class="col">
                        <div class="form-floating">
                            <select class="form-select">
                                <option value="1">information one</option>
                                <option value="2">information two</option>
                                <option value="3">information three</option>
                            </select>
                            <label for="floatingSelectGrid">More Info</label>
                        </div>
                    </div>
                </div>

                <div class="form-floating mt-4">
                    <textarea class="form-control" placeholder="Message" style="height: 100px"></textarea>
                    <label for="floatingTextarea2">Message</label>
                </div>

                <!-- bottone riutilizzabile   -->
                <div class="mt-4">
                    <AppButton buttonText="SEND" />
                </div>

            </div>

            <!-- colonna Vehicle Types   -->
            <div class="col">
                <h4>Example Inc.</h4>
                <p class="mt-3">Lorem ipsum dolor sit amet, consectetur adipisicing ai elit.</p>
                <p class="mt-3">Lorem ipsum dolor sit amet, consectetur adipisicing ai elit.</p>

                <!-- contatti   -->
                <div class="mt-4 contact">
                    <p><i class="icon fa-solid fa-phone"></i>+1(305)1234-5678</p>
                    <p><i class="icon fa-solid fa-envelope"></i>hello@example.com</p>
                    <p><i class="icon fa-solid fa-location-dot"></i>Main Avenue,987</p>
                    <!-- bottone riutilizzabile   -->
                    <AppButtonTran buttonText="VIEW MAP"/>

                </div>
            </div>
        </div>
    </section>
</template>


<style scoped lang="scss">
@use "./style/partials/variables" as *;
@use "./style/general.scss";

.container {
    padding-top: 5rem;
    padding-bottom: 5rem;
}

.title-bg {
    background-color: rgba($FountainBlue, 0.5);
    color: $BlueLagoon;
}

.icon{
    padding: .6rem;
    background-color: rgba($FountainBlue, 0.5);
    color: $BlueLagoon;
    border-radius: 50%;
    margin-right: .5rem;
}
.contact p{
    color: $BlueLagoon;
}

</style>