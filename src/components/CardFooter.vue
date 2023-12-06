<script>

export default {
    props: {
        card: {
            type: String,

        }
    },
}
</script>


<template>
    <div class="card" style="width: 14rem;">
        <div class="card-body">
            <h4 class="card-title fw-bold"></h4>
            <ul>
                <li class="d-flex text-start">
                    <i class="icon fa-solid fa-chevron-right"></i>
                    <p class="mb-0"></p>
                </li>
            </ul>

        </div>
    </div>
</template>


<style scoped lang="scss">
@use "./style/partials/variables" as *;

.card{
    background-color: gray;
}
ul{
    list-style-type: none;
    padding: 0;
}
.icon{
    padding-right: .5rem;
    padding-top: .2rem;
}

</style> 