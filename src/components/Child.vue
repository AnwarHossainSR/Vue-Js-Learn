<template>
    <div>
        <h1>{{ user.name }}</h1>
        <h1>{{ user.email }}</h1>
        <h1>{{ data() }}</h1>
        <div v-html="tag"></div>
    </div>
</template>

<script>
    export default {
       name:'Child',
       props:{
           user:Object,
           data:Function
       },
       data(){
           return{
               tag:'<h1>Hello Tag</h1>'
           }
       } 
    }
</script>