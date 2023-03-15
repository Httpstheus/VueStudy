<template>
    <div>
        <ul>
        <li> <a href="#"></a>Home</li>
        <li> <a href="#"></a>Projetos</li>
        <li> <a href="#"></a>Contato</li>
    </ul>
    </div>
</template>

<script>
    export default {
        name: 'Header'
    }
</script>

<style scoped>
    ul {
        list-style: none;
        display: flex;
        background: red;
    }

    li{
        margin-right: 10px;
    }

    a {
        color: #000000;
        text-decoration: none;
        transition: .5s;
    }

    a:hover{ color: aquamarine;}
</style>