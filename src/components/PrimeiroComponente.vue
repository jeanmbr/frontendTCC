<template>
    <h1>Primeiro Componente</h1>
    <p>Meu nome é {{ nome }} e trabalho como {{ profissao }}</p>
</template>

<script>
    export default {
        name: 'PrimeiroComponente',
        data() {
            return {
                nome: 'X',
                profissao: 'Programador'
            }
        }
    }
</script>
