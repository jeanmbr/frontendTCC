<template>
    <p v-if="esta_trabalhando">
        Estou trabalhando no momento.
    </p>
    <p v-else>
        Estou em busca de emprego no momento.
    </p>
    <p>
        Utilizo as seguintes tecnologias:
    </p>
    <ul>
        <li>Vue.js</li>
        <li>JavaScript</li>
        <li>HTML</li>
    </ul>
    <p v-show="mostrar_email">
        Mande uma mensagem para : {{ email }}
    </p>
    <p>
        Para acessar meu site, basta clicar no link abaixo:
        <a v-bind:href="link" target="_blank">Meu Site</a>
    </p>
</template>

<script>
    export default {
        name: 'InfoPessoa',
        data(){
            return{
                mostrar_email: true,
                email: 'jeanmachadobrasil@gmail.com',
                esta_trabalhando: false,
                link: 'https://github.com/jeanmbr'
            }
        }
    }
</script>
