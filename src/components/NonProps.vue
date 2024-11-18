<template>
    <div>

        <h3>Ayyan</h3>
        <h3>Reem</h3>
        <h3>Abdullah</h3>
        <h3 v-bind="$attrs">{{ name }}</h3>
    </div>


</template>

<script>
        export default{
            name:'NonProps',
            inheritAttrs:false,
            props:{
                name:String
            }
        }
</script>

<style scoped>
#main-comp{
    color: red;
}
</style>