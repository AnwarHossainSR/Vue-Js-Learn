<template>
    <div>
        
        <h1>Login</h1><br>
    
        <input type="text" name="email" v-model="email"><br>
    
        <input type="text" name="password" v-model="password"><br>
    
        <button v-on:click="getData">Submit</button>
    
    </div>
</template>

<script>
export default {
    name: 'Home',
    props: {
        name: String
    },
    data() {
        return {
            email:null,
            password:null
        }
    },
    methods: {
        getData() {
            alert(this.email +" "+this.password)
        }
    }
}
</script>

<style scoped>
h1 {
    color: darkolivegreen;
}
</style>
