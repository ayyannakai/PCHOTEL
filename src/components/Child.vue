<template>
    <button v-on:click="getUser(names)">click me</button>
</template>

<script>
    export default{
        name:'Child',
        data(){
            return{
                names:'ayyan'
            }
        },
        props:{
            getUser:Function
        }
        
    }
</script>