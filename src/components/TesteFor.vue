<template>
    <div class="teste-for">
        <h2>Teste For</h2>
        <ul>
            <li v-for="animal of animais" v-bind:key="animal.id">
                <img v-bind:src="animal.url" v-bind:alt="animal.nome"/>
            </li>
        </ul>
    </div>
        
</template>

<script>
export default {
    name: 'TesteFor',
    data(){
        return{
            animais:[
                {
                    id: 1,
                    nome: 'Gatinho',
                    url: 'https://p2.trrsf.com/image/fget/cf/600/400/images.terra.com/2020/08/14/o-gatinho-de-cada-signo-15721.jpeg'
                },
                {
                    id: 2,
                    nome: 'Cachorrinho',
                    url: 'https://escolaeducacao.com.br/wp-content/uploads/2022/01/Snowball-750x420.jpg'
                },
                {
                    id: 3,
                    nome: 'Cachorrinho',
                    url: 'https://escolaeducacao.com.br/wp-content/uploads/2022/01/Snowball-750x420.jpg'
                }
            ]
        }
    }
}
</script>

<style scoped>

</style>