<template>
    <div>
        <h1>Home Component</h1>
        <h3>Name : {{ name }}</h3>
        <p>Email : {{ email }}</p>
        <p>Address : {{ address }}</p>
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
                address:'Dhaka'
            }
        }
    }
</script>

<style scoped>
    h1{
        color: darkolivegreen;
    }
</style>
