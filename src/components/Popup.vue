<template>
    <div>
        <h5>This is Popup</h5>
        <button @click="$emit('close', 'Nay nay')">close popup</button>

    </div>
</template>

<script>
    export default {
        name:'Popup',
        emits:'close',
    }
</script>

<style scoped>

</style>