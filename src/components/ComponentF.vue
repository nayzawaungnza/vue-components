<template>
    <div>
        <h1>Component F</h1>
        <h2>Component F username {{ username }}</h2>
    </div>
</template>

<script>
    export default {
        name:'ComponentF',
        inject:['username'],
    }
</script>

<style scoped>

</style>