<script>

    export default{
        props:{
            handleClick: Function,
        }
    }
</script>

<template>
    <div id="botao" @click="handleClick">
        <p>Edit</p>
    </div>
</template>

<style scoped>

    #botao{
        width: 30px;
        height: 30px;
        border: 1px solid black;
        border-radius: 5px;
    }

    p{
        margin: 1px;
    }
</style>