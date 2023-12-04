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
   <button>{{buttonText}}</button>
</template>


<style scoped lang="scss">
@use "./style/partials/variables" as *;
button{
    background-color: $BlueChillVibrant;
    color: $White;
    border-radius: 5px;
    border: 0;
    padding: .5rem;


}
</style> 