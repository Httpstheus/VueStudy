<template>
    <form action="" @submit="enviarFormulario($event)">
        <div>
            <input type="text" v-model="name">
        </div>
        <div>
            <input type="text" v-model="email">
        </div>
        <div>
            <inputSubmit/>
        </div>


    </form>
</template>

<script>
 import inputText from './06 - inputText'
 import inputSubmit from './07 - Submit'

    export default {
        name: 'Form',
        components: {
            inputText,
            inputSubmit
        },
        data(){
            return{
                name: "",
                email: ""
            }
        },
        methods: { 
            enviarFormulario(e) {

                e.preventDefault()
                const name = this.name;
                const email = this.email;
            console.log("Formulário Enviado");
            console.log("O nome é " + name);
            console.log("O email é " + email);
        }
      
    }
}
</script>

<style scoped>
p{
    margin: 50px;
}
   
</style>
