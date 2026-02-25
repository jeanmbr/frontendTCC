<template>
    <img :src="avatar" :alt="descricao">
</template>

<script>
    export default{
        name: 'FotoGrafia',
        data(){
            return{
                avatar: "/img/java.png",
                descricao: "Logo do Java"
            }
        }
    }
</script>