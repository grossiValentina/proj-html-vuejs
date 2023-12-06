<script>

export default {
    props: {
        titleStyle: {
            type: String,

        }
    },
}
</script>


<template>
    <div class="d-flex">
        <h4 class="next ps-3 me-1">NEX</h4>
        <h4 class="title-gen">GEN</h4>
    </div>
</template>


<style scoped lang="scss">
@use "./style/partials/variables" as *;

.next {
    background-color: rgba($FountainBlue, 0.5);
    color: $BlueLagoon;
    border-top-left-radius: 15px;
    border-bottom-left-radius: 15px;
}
.title-gen{
    color: $White;
}

</style> 