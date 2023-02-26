<script>
import EditButton from '@/components/Botoes/EditButton.vue';
import DeleteButton from '@/components/Botoes/DeleteButton.vue';

    export default{
    data(){
        return{

        }
    },
    props: {
        user: Object,
    },
    components: { EditButton, DeleteButton },
    methods:{
        edit(){
            console.log(3);
        },
        deletar(){
            console.log(343);
        }
    }
}

</script>

<template>
    <div id="item">
        <div id="first">
            <h1>{{ user.username }}</h1>
            <div id="buttons">
                <EditButton :handle-click="edit" />
                <DeleteButton :handle-click="deletar" />
            </div>
        </div>
        <h3>{{ user.id }}</h3>
    </div>
</template>

<style scoped>

    #item{
        border: 2px solid black;
        border-radius: 15px;
        margin: 2.5%;
    }

    h1{
        margin-left: 2.5%;
        margin-top: 1%;
        margin-bottom: 1%;
    }

    h3{
        margin-left: 2.5%;
        margin-top: 1%;
        margin-bottom: 1%;
    }

    #first{
        display: flex;
        align-items: center;
        justify-content: space-between;
        border-bottom: 1px solid black;
    }

    #buttons{
        width: 10%;
        display: flex;
        align-items: center;
        justify-content: space-between;
        margin-right: 3%;
    }

</style>