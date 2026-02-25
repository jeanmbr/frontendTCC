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
    <div>
        <button @click="showEmail"> {{ textoBotao }} </button>
    </div>
    <p v-show="mostrar_email">
        Mande uma mensagem para : {{ email }}
    </p>
    <p>
        Para acessar meu site, basta clicar no link abaixo:
        <a v-bind:href="link" target="_blank">Meu Site</a>
        <FotoGrafia />
    </p>
</template>

<script>
    import FotoGrafia from './FotoGrafia.vue'

    export default {
        name: 'InfoPessoa',
        components:{
            FotoGrafia
        },
        data(){
            return{
                mostrar_email: false,
                email: 'jeanmachadobrasil@gmail.com',
                esta_trabalhando: false,
                link: 'https://github.com/jeanmbr',
                textoBotao: "Mostrar email"
            }
        },
        methods:{
            showEmail(){
                this.mostrar_email = !this.mostrar_email
                if (!this.mostrar_email) {
                    this.textoBotao = "Mostrar email"
                } else {
                    this.textoBotao = "Esconder email"
                }
            }
        }
    }
</script>
