<script>
import SidebarMenu from '@/components/sideBar/SidebarMenu.vue';
import ListagemComp from './Listagem/ListagemComp.vue';


export default{
    components: { ListagemComp, SidebarMenu }
}

</script>

<template>
    <div id="users">
        <SidebarMenu />
        <ListagemComp />
    </div>

</template>

<style scoped>


</style>