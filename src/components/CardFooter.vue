<script>

export default {
    props: {
        card: {
            title: String,
            list: Array,

        }
    },
}
</script>


<template>
    <div class="card" style="width: 14rem;">

        <div v-for="item in card" class="card-body">
            <h4 class="card-title fw-bold">{{ item.title }}</h4>
            <ul>
                <li v-for="arrayList in item.list" class="d-flex text-start">
                    <i class="icon fa-solid fa-chevron-right"></i>
                    <p class="mb-0">{{ arrayList }}</p>
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