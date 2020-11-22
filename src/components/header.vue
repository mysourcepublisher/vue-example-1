<template>
    <div id="header">
        <h1>{{ title }}</h1>
        <p id="users">Registered Users : {{value}}</p>
    </div>
</template>

<script>
export default {
    name : 'Header',
    props:{
        title:String,
        value:Number
    }
}
</script>

<style scoped>
    #header{
        font-family: Arial, Helvetica, sans-serif;
        display: flex;
        justify-content: space-between;
        color: #2e3c50;
        border-bottom: 2px solid rgba(0, 0, 0, 0.5);
        padding-left: 20px;
        padding-right: 20px;
    }
</style>