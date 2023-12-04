<script>
import AppList from "./AppList.vue";
import CardVehicle from "./CardVehicle.vue";

export default {
    data() {
        return {
            list: [
            {
                text: "lorem ipsum dolor"
            },
            {
                text: "adipisicing elit"
            },
            {
                text: "suscipit corrupti ipsa rem quo"
            },
            {
                text: "Laudantium atque temporibus"
            },
            {
                text: "blanditiis, cum voluptatum?"
            }
            ],

        }
    },
    components: {AppList, CardVehicle, }
}
</script>


<template>
    <section class="container">
        <div class="row">
            
            <!-- colonna Excellence in Transport  -->
            <div class="col-8 me-4">
                <h5>WHO WE ARE</h5>
                <div class="d-flex">
                    <h2 class="title-bg ps-2 pe-2"><i class="fa-regular fa-gem"></i>Exellence</h2>
                    <h2 class="ps-3">in Transport</h2>
                </div>
                <p class="pt-3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga, illo! Molestiae pariatur distinctio, laborum adipisci reprehenderit </p>  
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga, illo! Molestiae pariatur distinctio, laborum adipisci reprehenderit </p>  
                <div class="line-green">
                    <p class="font-italic ms-4 mb-0 pt-3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Culpa nulla perferendis dolorem praesentium. Officia, repellendus </p>
                </div>
                <p class="pt-3">Lorem ipsum dolor sit, amet consectetur adipisicing elit. </p>
                
                <!-- lista dinamica  -->
                <div>
                   <AppList :list="list"/>
                </div>
            </div>

            <!-- colonna Vehicle Types   -->
            <div class="col">
               <h4>Vehicle Types</h4>
               <CardVehicle />
            </div>

        </div>
        <div>

        </div>
    </section>
</template>


<style scoped lang="scss">
@use "./style/partials/variables" as *;
@use "./style/general.scss";

.container {
    padding-top: 5rem;
};
.title-bg{
    background-color: rgba($FountainBlue, 0.5);
    color: $BlueLagoon;
};
.line-green{
    border-left: 4px solid rgba($FountainBlue, 0.5);
    height: 5rem;
};
ul{
    margin-left: 12px;
    padding: 0;
}
</style>