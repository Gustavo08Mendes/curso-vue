<template>
    <div>
        <a href="#">Home</a>
        <a href="#">Conta</a>
        <a href="#">Links</a>
    </div>
</template>

<script>
    export default {
        name: 'Header'
    }
</script>

<style scoped>
    div {
        background-color: #1a1a1a;
        padding: 5px 10px;
    }
    a{
        text-decoration: none;
        color: #fff;
        padding: 0 10px;
        font-weight: bold;
        font-family: Arial, Helvetica, sans-serif;
        transition: .5s;
    }
    a:hover {
        color: #ffbb33;
    }
</style>