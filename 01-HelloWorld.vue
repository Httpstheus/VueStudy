<template>
 <div>
  <h1>Olá Vue!</h1>
  <p>Meu nome é {{ nome }} e trabalho como {{ profissao }}</p>
  <MultiplosEventos/>
 </div>
</template>

<script>
 
  import MultiplosEventos from './10 - MultiplosEventos';

export default {


    name: 'HelloWorld',
    components: {
      MultiplosEventos
    },
    data(){
        return {
          nome: "Matheus",
          profissao: "Programador"
        }
 }
}
</script>  
