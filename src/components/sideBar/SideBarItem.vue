<script>

    export default{
        name:"SideBarItem",
        data(){
            
        },
        components: {
        },
        props:{
            title : String,
            clickHandler: Function
        },
        
    }
</script>

<template>
    <div id="item" @click="clickHandler">
        <span>{{title}}</span>
    </div>
</template>

<style scoped>
    #item{
        width: 85%;
        height: 5%;
        display: flex;
        justify-content: center;
        align-items: center;
        margin: 20px;
        border: 2px solid black;
        border-radius: 15px;
    }
    span{
        font-size: 30px;
        user-select: none;
    }
</style>