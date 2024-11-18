<template>

    <h1 :class="classes">carlos sainz</h1>
    <button v-on:click="colorful=!colorful">color change</button>
</template>

<script>
    export default{
        name:'ClassBinding',
        data(){
            return{
                colorful:true
            }
        },computed:{
            classes(){
                return{
                    red:this.colorful,
                    border:true
                }
            }
        }
    }
</script>

<style scoped>
  
    .border{
        background-color: yellow;
        
    }
    .red{
        color: red;
    }
</style>