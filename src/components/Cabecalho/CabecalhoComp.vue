
<script>
    export default {
        props:{
            title: String,
        }
    }
</script>

<template>
        <div id="headerContainer">
            <h1>{{ title }}</h1>
        </div>

</template>

<style scoped>

    #headerContainer{
        height: 20%;
        width: 100%;
        display: flex;
        align-items: flex-end;
    }

    h1{
        margin-left: 5%;
        margin-bottom: 0%;
        font-size: 350%;
    }

</style>