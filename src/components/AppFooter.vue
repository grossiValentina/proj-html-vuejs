<script>
import AppButtonTran from "./AppButtonTran.vue";
import Title from "./Title.vue";
import Contacts from "./Contacts.vue";

export default {
    data() {
        return {
            
        }
    },
    components: { AppButtonTran, Title, Contacts }
    
}
</script>

<template>
  <section class="wrapper">
    <div class="container">
        <div class="row row-cols-4">
            <div class="col">
                
                 <!-- titolo riutilizzabile  -->
                <Title  titleStyle="titleStyle" />
                
                <p>Lorem ipsum dolor sit amet consectetur</p>

                 <!-- contatti riutilizzabili  -->
                 <div class="mt-4 mb-4">
                    <Contacts contact="contact"/>
                    <p><i class="p-1 fa-solid fa-location-dot"></i>Main Avenue,987</p>
                 </div>

                 <!-- bottone riutilizzabile  -->
                <AppButtonTran buttonText="GET IN TOUCH"/>
            </div>
             
             <!-- card con lista  -->
            <div class="col">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Sunt culpa, aut quae ut, voluptatibus animi aliquid iusto recusandae voluptatum obcaecati autem! Animi, id quia neque ad quos eligendi odit iusto.</div>

            <div class="col">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quos voluptatum voluptatibus voluptatem error quidem numquam magnam voluptates doloremque natus. Laborum facilis animi voluptate reiciendis doloremque eius exercitationem aliquam iure qui!</div>

            <div class="col">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Suscipit, quaerat voluptas assumenda placeat natus iusto possimus ab debitis adipisci amet maiores mollitia nostrum similique, nihil nemo explicabo? Dolore, maiores accusantium?</div>
        </div>

    </div>

  </section> 
</template>


<style scoped lang="scss">
@use "./style/partials/variables" as *;
@use "./style/general.scss";

.wrapper{
    background-color: pink;
}
.container{
    padding-top: 5rem;
    padding-bottom: 5rem;
}

p{
    color: $White;
}
</style>