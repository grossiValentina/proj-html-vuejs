<script>
import AppHeader from "./components/AppHeader.vue";
import AppButton from "./components/AppButton.vue";
import SectionMain1 from "./components/SectionMain1.vue";
import SectionMain2 from "./components/SectionMain2.vue";
import AppFooter from "./components/AppFooter.vue";
import { store } from "./store.js";


export default {
  

  methods: {
    

    },

  components :{
    AppHeader,
    AppButton,
    SectionMain1,
    SectionMain2,
    AppFooter,
},
}

</script>

<template>
<AppHeader />
<AppButton />
<SectionMain1/>
<SectionMain2 />
<AppFooter />

 
</template>

<style lang="scss">
@use "./components/style/general.scss";
@import "@fortawesome/fontawesome-free/css/all.css";

</style>
