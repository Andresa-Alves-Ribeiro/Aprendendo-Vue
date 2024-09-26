<template>
    <div class="componente">
        <h1>Componente com Data Binding</h1>
        <!-- <input type="text" v-bind:value="valor"></input>    ONE WAY DATA BINDING  -->
        <p>{{ valor }}</p>

        <!-- <input type="text" v-bind:value="valor" v-on:input="(e) => valor = e.target.value" /> TWO WAY DATA BINDING -->
        <!-- <input type="text" :value="valor" @input="(e) => valor = e.target.value" /> FORMA SIMPLIFICADA -->

        <input type="text" v-model="valor" /> <!-- FORMA MAIS USADA BIDIRECIONAL -->
    </div>
</template>

<script setup>
import { ref } from 'vue';

const valor = ref('Teste de valor'); 
</script>

<!-- v.bind:value = Para pegar valores definidos em função


 v-on:input = Para mandar o valor digitado no input para o const
-->