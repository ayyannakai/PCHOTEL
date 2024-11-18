<template>
    <h3>{{ (dollars*rupees) - discount }}</h3>
    <h3>{{ getValue }}</h3>

</template>

<script>
    export default{
        name:'ComputedProperty',
        data(){
            return{
                dollars:100,
                rupees:300,
                discount:1000
            }

        },computed:{
            getValue(){
                return (this.dollars*this.rupees) - this.discount
            }
        }
    }
</script>

<!-- functions in computed are better than those in methods -->