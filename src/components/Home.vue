<template>
    <div>
        
        <h1>Login</h1><br>
        <label for="java">Java</label>
        <input type="checkbox" id="java" value="Java" v-model="technology">
        <label for="php">Php</label>
        <input type="checkbox" id="php" value="Php" v-model="technology">
        <label for="python">Python</label>
        <input type="checkbox" id="python" value="Python" v-model="technology"><br>

        <h1>Who i am</h1>
        <label for="developer">Developer</label>
        <input type="radio" name="profession" value="Developer" id="developer" v-model="who">
        <label for="student">Student</label>
        <input type="radio" name="profession" value="Student" id="student" v-model="who">
        <label for="business">Business man</label>
        <input type="radio" name="profession" value="Businessman" id="business" v-model="who"><br><br>

        <h3>Technologies : {{ technology }}</h3><br>
         <h3>Who i am : {{ who }}</h3>
    
    </div>
</template>

<script>
export default {
    name: 'Home',
    data() {
        return {
            technology:[],
            who:null
        }
    }
}
</script>

<style scoped>
h1 {
    color: darkolivegreen;
}
</style>
