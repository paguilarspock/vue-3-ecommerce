<script setup lang="ts">

    import {onMounted, ref} from 'vue'
    const count = ref(0);

    function aumentar(){

        count.value += 1;

    }


    onMounted(function (){

        console.log('El valor incial del contador es ' + count.value);

    });


</script>


<template>
    <h1>Hola soy la version con Composition API</h1>
    <h1>Contador: {{ count }}</h1>
    <button @click="aumentar">Incrementar Button</button>
</template>