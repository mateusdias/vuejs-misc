<template>
    <div id="assine">
        <h1>Assine o nosso serviço de música</h1>
        <p>Preencha seus dados</p>
        <input v-model="nome" placeholder="Seu nome"><br/>
        <input v-model="email" placeholder="Email"><br/>
        <textarea v-model="textotermos" placeholder="Termos de serviço: Textão" readonly/><br/>
        <input type="checkbox" id="termos-check" v-model="checktermos" />
        <label for="termos-check">Aceito os termos</label><br/>
        <v-btn class="button">Contratar</v-btn>
        <hr>
        <h2>Dados que vc preencheu:</h2>
        <p>Nome: {{ this.nome }} </p>
    </div>
</template>

<script>
export default {
    methods: {
        
    }
}
</script>

<style scoped>
#assine{
    color: gray;
}

</style>