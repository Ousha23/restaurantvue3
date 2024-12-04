<template>
    <div>
        <h4>{{ year }}</h4>
        <h5>{{ title }}</h5>
        <P>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Velit nam cumque vero, dolorem deleniti libero numquam magnam nemo quisquam est. Minus optio accusamus porro repudiandae sed, necessitatibus illo perferendis fugiat?</P>
    </div>
</template>
<style scoped>
    h4 {
        color: burlywood;
        text-decoration: solid;
        padding: 10px;
    }
    h5 {
        font-family: Rami;
        font-size: larger;
        padding: 10px;
    }

    p {
        padding: 10px;
    }
</style>
<script setup>
    const props = defineProps({
        title : String,
        year : String,
    });
    
</script>