<template>
    <div class="contador-desafio">
        <p><strong>Contador: </strong>{{contador}}</p>
        <button @click="removeUm">-</button>
        <button @click="somarUm">+</button>
    </div>
</template>

<script>
export default {
    name: 'ContadorDesafio',
    data(){
        return{
            contador: 0
        }
    },
    methods: {
        removeUm(){
            this.contador--;
        },
        somarUm() {
            this.contador++;
        }
    }
}
</script>

<style scoped>

</style>