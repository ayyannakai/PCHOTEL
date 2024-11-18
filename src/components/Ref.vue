<template>
    <input type="text" ref="input">
    <button v-on:click="getInput">Input</button>
</template>

<script>
    export default{
        name:'Ref',
        methods:{
            getInput(){
                console.log(this.$refs.input.value)
                this.$refs.input.value = ''
                
            }
        }
    }
</script>