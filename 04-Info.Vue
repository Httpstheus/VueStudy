<template>

    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento</p>
        <p v-else>Estou em busca de novas oportunidades</p>
        <p>Utilizo as seguintes tecnologias</p>
        <ul>
            <li>Javascript</li>
            <li>PHP</li>
            <li>SQL</li>
        </ul>
        <p v-if=" 4 > 2"> 4 é maior que 2</p>
        <p v-else> 4 não é maior</p>
        <p v-show="mostrar_email">Entre em contato pelo email: {{ email }}</p>
        <p>Para acessar meu portfólio basta <a v-bind:href="meu_link" target="_blank">clique aqui</a></p>
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
        data() {
            return {
                esta_trabalhando: false,
                mostrar_email: true,
                email: 'matheusrodrigues@mundialeditora.com',
                meu_link: 'https://matheusrodriguesdev.vercel.app/'
            }
        }
    }
</script>
