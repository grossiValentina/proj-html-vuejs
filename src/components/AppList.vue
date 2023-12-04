<script>

export default {
   
    props: {
        list: {
            type: Array,
        },
    }
} 

</script>


<template>
    <ul>
        <li v-for="item in list" :key="item.text" >{{ item.text }}</li>
    </ul>
</template>


<style scoped lang="scss">
@use "./style/partials/variables" as *;
</style> 