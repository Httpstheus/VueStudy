<template>
    <div>
        <h2>Esta é a descrição da pessoa {{ nome }}</h2>
        <Info/>
        <Form/>
    </div>
</template>

<script>
    import Info from './04 - Info'
    import Form from './05 - Form'
    
    export default {
        name: 'Pessoa',
        components: {
            Info, Form
        },
        data() {
            return {
                nome: "Matheus"
            }
        }
    }
</script>
