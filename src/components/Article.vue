<template>
    <div>
        <h2>Article Component</h2>
        <h3>{{ title }} -- Like - {{ likes }} -- Published is {{ isPublished ? 'Yes':'No' }}</h3>

    </div>
</template>

<script>
    export default {
        name:'Article',
        props:{
            title:{
                type:String,
                required:true,
                default:'Article Default Title'
            },
            likes:Number,
            isPublished:Boolean,
        },
    }
</script>

<style scoped>

</style>