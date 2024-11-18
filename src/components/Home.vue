<template>
    <!-- <h1>hi my name is ayyan</h1>
    <h2>{{ person }}</h2>
    <Child :getUser="getUserName"/>
    <Ref/> -->
    <!-- <NonProps name="araiz" id="main-comp"/>
      -->
    <!-- <ComputedProperty/> -->
     <Watchers/>

    <!-- <input type="text" v-model="num">
    <h1>{{ num }}</h1>
    <button v-on:click="getCount()">click me {{ count }}</button> <br/><br/>
    <input type="email" placeholder="email" v-model="email"> <br/>  <br/>
    <input type="password" placeholder="password" v-model="password"><br/><br/>
    <button v-on:click="submit">submit</button> -->
</template>

<script>
import Ref from './Ref.vue';
import Child from './Child.vue';
import NonProps from './NonProps.vue';
import ComputedProperty from './ComputedProperty.vue';
import Watchers from './Watchers.vue';


export default {
    name:'name',
    data(){
        return{
            person:''
        }
    },

    components:{
        Child,
        Ref,
        NonProps,
        ComputedProperty,
        Watchers
    },methods:{
        getUserName(name){
            this.person = name
        }

    }
    // ,methods:{
    //     getName(){
    //         return{

    //         }
    //     }
    // }
    // data(){
    //     return{
    //         number:55,
    //         count:0,
    //         email:null,
    //         password:null,
    //         getFunc:function(num){
    //             return num
    //         },
    //         num:0
    //     }
    // },
    // methods:{
    //     getEmail(){
    //         return{
    //             name:'ayyan',
    //             email:"ayyannakai7@gmail.com",
    //             number:this.number
    //         }
    //     },
    //     getCount(){
    //         return this.count++
    //     },
    //     submit(){
    //         console.log(this.email,this.password)
    //         this.email= null
    //         this.password = null
    //     }
    // }

}

</script>

<style scoped>
h1{
    color: rgb(57, 145, 57);
}
</style>