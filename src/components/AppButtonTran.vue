<script>

export default {
   props: {
    buttonText:{
        type: String,
       
    }
   },
}
</script>


<template>
   <button class="btn btn-outline-dark">{{buttonText}}</button>
</template>


<style scoped lang="scss">
@use "./style/partials/variables" as *;

button{
    border-color: $BlueChillVibrant;
    color: $BlueChillVibrant;
    border-radius: 5px;
    border: 1px solid;
    padding: .5rem;

}
</style> 