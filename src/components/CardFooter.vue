<script>

export default {
    props: {
        firstCard: {
            type: Object,
        },

        secondCard: {
            type: Object,
        },

        thirdCard: {
            type: Object,
        },
    }
}
</script>

<template>
    <div class="col">

        <div v-for="item in firstCard" class="card" style="width: 14rem;">

            <div class="card-body">
                <h4 class="card-title fw-bold">{{ item.title }}</h4>
                <ul>
                    <li v-for="item in firstCard" class="d-flex text-start">
                        <i class="icon fa-solid fa-chevron-right"></i>
                        <p class="mb-0">{{ item.list }}</p>
                    </li>
                </ul>

            </div>
        </div>

    </div>

</template>


<style scoped lang="scss">
@use "./style/partials/variables" as *;

.card {
    background-color: grey;
}

ul {
    list-style-type: none;
    padding: 0;
}

.icon {
    padding-right: .5rem;
    padding-top: .2rem;
}

;
</style> 