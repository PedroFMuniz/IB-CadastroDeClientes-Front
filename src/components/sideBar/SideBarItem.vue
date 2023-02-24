<script>

    import SvgIcon from '@jamescoyle/vue-icon';
    import { mdiAccountCircle, mdiShoppingOutline, mdiAccountCashOutline } from '@mdi/js';

    export default{
        name:"SideBarItem",
        data(){
            
        },
        components: {
            SvgIcon
        },
        props:{
            title : String,
            path: mdiAccountCircle || mdiShoppingOutline || mdiAccountCashOutline,
            clickHandler: Function
        },
        
    }
</script>

<template>
    <div id="item" @click="clickHandler">
        <svg-icon type="mdi" :path=path />
        <span>{{title}}</span>
    </div>
</template>

<style scoped>
    #item{
        width: 70%;
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