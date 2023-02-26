<script>

import CabecalhoComp from '@/components/Cabecalho/CabecalhoComp.vue';
import ItemComp from './ItemComp.vue';

    export default{
        components:{
    CabecalhoComp,
    ItemComp
},
        data(){
            return{
                HeaderTitle: "Usuários",
                users: [
                    {
                        id: 0,
                        username: 'Pedro',
                    },
                    {
                        id: 1,
                        username: 'Pedro',
                    },
                    {
                        id: 2,
                        username: 'Pedro',
                    },
                    {
                        id: 3,
                        username: 'Pedro',
                    },
                    {
                        id: 4,
                        username: 'Pedro',
                    },
                    {
                        id: 5,
                        username: 'Pedro',
                    },
                    {
                        id: 6,
                        username: 'Pedro',
                    },
                    {
                        id: 7,
                        username: 'Pedro',
                    },
                    {
                        id: 8,
                        username: 'Pedro',
                    },
                    {
                        id: 9,
                        username: 'Pedro',
                    },
                    {
                        id: 10,
                        username: 'Pedro',
                    },
                    {
                        id: 11,
                        username: 'Pedro',
                    },
                    {
                        id: 12,
                        username: 'Pedro',
                    }
                ]
            }
        }
    }
</script>

<template>
    <div id="listagem">
        <CabecalhoComp :title="HeaderTitle" />
        <div id="listagemInterna">
            <ItemComp v-for="user in users" :key="user.id" :user="user" />
        </div>
    </div>
</template>

<style scoped>

#listagem{
  position: absolute;
  width: 60%;
  height: 100%;
  left: 25%;
}

#listagemInterna{
    border: 2px solid black;
    border-radius: 5px;
}
</style>