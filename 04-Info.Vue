<template>

<div>
    <p>{{ compEmail }}</p>
        <p v-if="esta_trabalhando">Estou trabalhando no momento</p>
        <p v-else>Estou em busca de novas oportunidades</p>
        <p>Utilizo as seguintes tecnologias para backend </p>
        <ul>
            <li v-for="(technology, index) in backend_tecnologies" v-bind:key="index" >{{ technology }}</li>
        </ul>
        <p>Utilizo as seguintes tecnologias para front-end</p>
        <ul>
            <li v-for="technology in frontend_tecnologies">
                {{ technology.language }}
            </li>
        </ul>
        <div>
                <button @click="showEmail"> {{ textoBotao }}</button>
        </div>
        <p v-if=" 4 > 2"> 4 é maior que 2</p>
        <p v-else> 4 não é maior</p>
        <p v-show="mostrar_email">Entre em contato pelo email: {{ email }}</p>
        <p class="p-text">Para acessar meu portfólio basta <a v-bind:href="meu_link" target="_blank">clique aqui</a></p>
        <Picture/>
</div>

</template>


<script>
  import Picture from './08 - Picture'
    export default {
        name: 'Info',
        components: {
            Picture
        },
        props: {
            compEmail: string
        },
        data() {
            return {
                esta_trabalhando: false,
                mostrar_email: false,
                email: 'matheus@gmail.com',
                meu_link: 'https://matheusrodriguesdev.vercel.app/',
                textoBotao: 'mostrar email',
                backend_tecnologies: ['JavaScript', 'PHP', 'Python'],
                frontend_tecnologies: [
                    {id: 1, language: 'HTML'},
                    {id: 2, language: 'CSS'},
                    {id: 3, language: 'JS'}
                ]
            }
        },
        methods: {
            showEmail(){
                this.mostrar_email = !this.mostrar_email
                if(!this.mostrar_email) {
                    this.textoBotao ='Mostrar Email'
                } else {
                    this.textoBotao = 'Esconder Email'
                }
            }
        }
    }

    </script>
