<template>
    <div>
        <h1>Home Component</h1>
        <h3>Name : {{ name }}</h3>
        <p>Email : {{ email }}</p>
        <p>Address : {{ address }}</p>
        <p>Method Name : {{ getname() }}</p><br>
        <button v-on:click="increment()">Click</button>
        <h1>{{ count }}</h1><br>
        <input type="text" v-model="count">
        <h1>{{ count }}</h1><br>
    </div>
</template>

<script>
    export default {
        name:'Home',
        props:{
            name:String
        },
        data(){
            return{
                email:'mahedianwar@Gmail.com',
                address:'Dhaka',
                count:0
            }
        },
        methods:{
            getname(){
                return this.name
            },
            increment(){
                this.count++
            }
        }
    }
</script>

<style scoped>
    h1{
        color: darkolivegreen;
    }
</style>
