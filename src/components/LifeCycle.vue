<template>
    <h1>Meu nome é: {{ nome }}</h1>
</template>

<script>

    export default {
        name: 'LifeCycle',
        data(){
            return{
                nome: 'Não definido'
            }
        },
        created(){
            setTimeout(() => {
                this.nome = 'Pedro'
            }, 1000)
        },
        mounted(){
            setTimeout(() => {
                this.nome = 'Jean'
            }, 2000)
        }
    }
</script>