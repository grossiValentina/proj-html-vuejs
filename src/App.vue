<script>
import AppHeader from "./components/AppHeader.vue";
import AppButton from "./components/AppButton.vue";
import SectionExellence from "./components/SectionExellence.vue";
import SectionServices from "./components/SectionServices.vue";
import SectionLogistical from "./components/SectionLogistical.vue";
import SectionResults from "./components/SectionResults.vue";
import SectionTrusted from "./components/SectionTrusted.vue";
import SectionMessage from "./components/SectionMessage.vue";
import AppFooter from "./components/AppFooter.vue";


export default {
  

  methods: {
    

    },

  components :{
    AppHeader,
    AppButton,
    SectionExellence,
    SectionServices,
    SectionLogistical,
    SectionResults,
    SectionTrusted,
    SectionMessage,
    AppFooter,
},
}

</script>

<template>

<AppHeader />
<AppButton />
<SectionExellence/>
<SectionServices />
<SectionLogistical />
<SectionResults />
<SectionTrusted />
<SectionMessage />
<AppFooter />

</template>

<style lang="scss">
@use "./components/style/general.scss";
@import "@fortawesome/fontawesome-free/css/all.css";

</style>
