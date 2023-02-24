<script>

import CabecalhoComp from '../Cabecalho/CabecalhoComp.vue';

    export default{
        components:{
            CabecalhoComp,
        },
        data(){
            return{
                HeaderTitle: "Consultoras",
            }
        }
    }
</script>

<template>
    <div id="listagem">
        <CabecalhoComp :title="HeaderTitle" />
    </div>
</template>

<style scoped>

#listagem{
  position: absolute;
  width: 60%;
  height: 100%;
  left: 25%;
  background-color: red;
}
</style>