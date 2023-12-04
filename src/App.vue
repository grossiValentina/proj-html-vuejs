<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";
import { store } from "./store.js";


export default {
  data() {
    return {
      store
    };
  },
    
  

  methods: {
    

    },

  components :{
      AppHeader,
      AppMain,
      AppFooter,
    
}
}

</script>

<template>
<AppHeader />
<AppMain />
<AppFooter />

 
</template>

<style lang="scss">
@use "./components/style/general.scss";
@import "@fortawesome/fontawesome-free/css/all.css";

</style>
