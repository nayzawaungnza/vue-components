<template>
    <div>
        <h5>This is Popup</h5>
        <input type="text" v-model="name" />
        <button @click="$emit('close', name)">close popup</button>

    </div>
</template>

<script>
    export default {
        name:'Popup',
        emits:{
            close:(name) => {
                if(!name){
                    return false
                }else{
                    return true
                }
            }
        },
        data(){
            return{
                name:'',
            }
        }
    }
</script>

<style scoped>

</style>