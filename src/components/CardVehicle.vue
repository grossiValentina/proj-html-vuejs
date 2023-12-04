<script>

export default {
    props: {
        vehicleType: {
            type: Array,
            default: () => [
            {
                size: "Light",
                maxWh: "Max Weigth 1200 kg"
            },
            {
                size: "Light",
                maxWh: "Max Weigth 6000 kg"
            },
            {
                size: "Light",
                maxWh: "Max Weigth 24000 kg"
            }
        ]
    },
}
}

</script>


<template>
    <div v-for="(item, index) in vehicleTypes" :key="index" 
    class="my-card" style="max-width: 250px;">
        <div class="row">
            <div class="col-md-4">
                <img src="../assets/img/truck-1.png"  alt="...">
            </div>
            <div class="col-md-8">
                <div class="card-content pb-0">
                    <h4 class="title mb-0">{{ vehicleType.size }}</h4>
                    <p class="text"><small class="text-muted">{{ vehicleType.maxWh }} </small></p>
                </div>
            </div>
        </div>
    </div>
</template>


<style scoped lang="scss">
@use "./style/partials/variables" as *;
.my-card{
  border-bottom: 1px solid $MidGray;   
};

img{
    padding: .3rem;
    background-color:  rgba($FountainBlue, 0.3);
    width: 5rem;
    margin-top: .5rem;
}
.card-content{
    padding: .5rem;
}
</style> 