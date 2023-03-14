<template>
    <img :src="avatar" :alt="descricao">
</template>    

<script>
    export default {
        name: 'Picture',
        data(){
            return{
                avatar: "https://www.seekpng.com/png/detail/983-9833965_icon-people-people-icon-black-png.png",
                descricao: 'Icone pessoa'
            }
        }
    }
</script>