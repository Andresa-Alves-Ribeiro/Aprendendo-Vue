<template>
    <div class="componente">
        <h1>Componente Com Dados Reativos Primitivos</h1>

        <p>Nome: {{ nome }} | Idade: {{ idade }}</p>

        <button v-on:click="fazerAniversario">Fazer Aniversário</button>
        <button @click="mudarNome">Mudar Nome</button>
    </div>
</template>

<script setup>
    // Definindo dados reativos

    import { ref } from 'vue';

    // PODE USAR CONST PRA MUDAR PQ ESTA SE REFERINDO AO OBJETO E NÃO AO VALOR

    const nome = ref("Ana")
    const idade = ref(29)

    function fazerAniversario() {
        idade.value += 1
    }

    function mudarNome() {
        nome.value = "Maria"
    }
</script>