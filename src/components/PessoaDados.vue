<template>
    <h2>Esta é a descrição da pessoa: {{ nome }}</h2>
    <InfoPessoa />
</template>

<script>
import InfoPessoa from './InfoPessoa.vue';
export default {
    name: 'PessoaDados',
    components:{
        InfoPessoa,
    },
    data() {
        return {
            nome: 'Jean',
        }
    }
}
</script>