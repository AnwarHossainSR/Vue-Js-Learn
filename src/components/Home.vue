<template>
    <child :user="user" :data="getData" />
</template>

<script>
import Child from './Child.vue'
export default {
  components: { Child },
    name: 'Home',
    data() {
        return {
            user:{
                name:'Mahedi Hasan',
                email:'mahedisr@gmail.com'
            }
        }
    },
    methods:{
        getData(){
            alert('hello')
        }
    }
}
</script>

<style scoped>
h1 {
    color: darkolivegreen;
}
</style>
