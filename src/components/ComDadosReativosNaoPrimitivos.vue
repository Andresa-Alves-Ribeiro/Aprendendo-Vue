<template>
    <div class="componente">
        <h1>Componente Com Dados Reativos Não Primitivos</h1>

        <p>Nome: {{ pessoa.nome }} | Idade: {{ pessoa.idade }}</p>

        <button @click="fazerAniversario">Fazer Aniversário</button>
        <button @click="mudarNome">Mudar Nome</button>
    </div>
</template>

<script setup>
    // Definindo dados reativos

    import { reactive } from 'vue';

    const pessoa = reactive({nome: "Maria", idade: 36})

    function fazerAniversario() {
        pessoa.idade += 1
    }

    function mudarNome() {
        pessoa.nome = "Bruna"
    }
</script>