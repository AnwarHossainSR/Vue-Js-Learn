<template>
    <div>
        <h1 v-if="show">If condition</h1>
        <h1 v-else>Else condition</h1>

        <button v-on:click="show=!show">Toggle</button>
    </div>
</template>

<script>
export default {
    name: 'Home',
    data() {
        return {
            show:false
        }
    }
}
</script>

<style scoped>
h1 {
    color: darkolivegreen;
}
</style>
