<template>
    <div><!-- 
        <h1>For loop</h1><br>
        <ul v-for="item in data" :key="item">
            {{ item }}
        </ul><br> -->
        <h1>For loop</h1><br>
        <ul v-for="item in object" :key="item.id">
            <ul>
                Name: {{ item.name }}
                Email: {{ item.email }}
            </ul><br>
        </ul>
        
    </div>
</template>

<script>
export default {
    name: 'Home',
    data() {
        return {
            object:[
                {
                    id:1,
                    name:'Maheid Hasan',
                    email:'mahedi@gmail.com'
                },{
                    id:2,
                    name:'Sultan Ahmed',
                    email:'sultan@gmail.com'
                }
            ]
        }
    }
}
</script>

<style scoped>
h1 {
    color: darkolivegreen;
}
</style>
