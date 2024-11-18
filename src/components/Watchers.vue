<template>
    <h3>
        PC HOTEL KA MALIK GANDU HAI

    </h3>
    <!-- <button v-on:click="count=count+1">+</button>
    <button v-on:click="count = count - 1">-</button> -->
</template>


<script>
    export default{
        name:'Watchers',
        data(){
            return{
                count:0
            }
        },
        watch:{
            count(val,prev){
                if( val>5 && val>prev){

                    alert('stop counting')
                }
            }
        }
    }
</script>