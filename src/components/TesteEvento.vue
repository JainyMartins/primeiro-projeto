<template>
    <div class="teste-evento">
        <h2>Teste Evento</h2>
        <p @click="deixarMaiuscula">{{mensagem}}</p>
    </div>
</template>

<script>
export default {
    name: 'TesteEvento',
    data() {
        return {
            mensagem: 'O rato roeu a roupa do rei de Roma'
        }
    },
    methods: {
        deixarMaiuscula(){
            this.mensagem = this.mensagem.toUpperCase();
        },
        deixarMinuscula(){
            this.mensagem = this.mensagem.toLocaleLowerCase();
        }
    }
}
</script>

<style scoped>

</style>