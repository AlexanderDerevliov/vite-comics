<script>
import AppHeader from './components/AppHeader.vue';
import AppContent from './components/AppContent.vue';
import AppLogos from './components/AppLogos.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  components: {
    AppHeader,
    AppContent,
    AppLogos,
    AppFooter,
    
},
  data (){
    return{
          
    }
  }
}
</script>

<template>
  
 <AppHeader />
 <AppContent />
 <AppLogos />
 <AppFooter />

</template>

<style lang="scss">
@use "./style/general.scss";


</style>
