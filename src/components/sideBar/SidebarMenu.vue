<template>
    <div id="containerMenu">
            <img src="../../assets/logo_temp.jpg" />
            <SideBarItem v-for="option in options" :key="option.id" :title="option.title" :path="option.icon" :clickHandler="aumentar" />
            <h3>{{ count }}</h3>
    </div>
</template>

<script>
import SideBarItem from './SideBarItem.vue';
import { mdiAccountCircle, mdiShoppingOutline, mdiAccountCashOutline } from '@mdi/js';

    export default{
    data(){
        return{
        options: [{
            id: 0,
            title: "Usuários",
            icon: mdiAccountCircle,
        },{
            id: 1,
            title: "Consultoras",
            icon: mdiShoppingOutline,
        },{
            id: 2,
            title:"Clientes",
            icon: mdiAccountCashOutline,
        }],
        count: 0,
        }
    },
    methods:{
        aumentar(){
            this.count++;
        }
    },

    components: { SideBarItem }
}

</script>

<style scoped>
    #containerMenu{
        position: fixed;
        margin-left: 7%;
        display: flex;
        align-items: center;
        flex-direction: column;
        width: 15%;
        height: 100%;
    }

    img{
        margin-top: 5%;
        border-radius: 100px;
    }
</style>