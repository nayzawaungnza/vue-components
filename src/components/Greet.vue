<template>
    <div>
<h1>hello {{ name }} a, k, a {{ heroName }}</h1>
    </div>
</template>

<script>
    export default {
        name:'Greet',
        props:['name','heroName'],
    }
</script>

<style scoped>

</style>