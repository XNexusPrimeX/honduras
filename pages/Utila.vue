<script lang="ts">
import Vue from 'vue';
import Section from '../components/Section.vue';

export default Vue.extend({
    name: 'Útila',
    components: {
        Section
    },
    data: () => ({
        image: 'utila.jpg',
        author: {
            name: 'Gabrielly Navarro Bastos',
            pic: 'https://pps.whatsapp.net/v/t61.24694-24/301435344_1410367002805366_7838172227822681169_n.jpg?ccb=11-4&oh=01_AVxaOqxUfrG2UR7iZZo7uasLrlRO7GgvSG38m1DmftJmlg&oe=63202DBD'
        }
    })
})
</script>

<template>
    <Section :image="image" :author="author" >
        <p>Útila es una isla hondureña en el departamento de Islas de la Bahía. Es una de las tres islas principales de este departamento insular y uno de sus cuatro municipios. Se encuentra a solo 30 km de la costa norte de Honduras y tiene un área de 49,3 km², 11 km de ancho y 4 km en su punto más angosto.</p>
        <p>El idioma oficial, como en el resto de Honduras, es el español, aunque también se habla inglés, principalmente por la presencia de turistas.</p>
        <p>La segunda cadena de arrecifes más grande del mundo se extiende por las Islas de la Bahía donde la vida marina es rica y abundante, aunándose a ello aguas cristalinas y una visibilidad de hasta 500 m, haciendo de Útila uno de los mejores lugares para el buceo, además ser considerado uno de los lugares más baratos del mundo para estudiar y obtener una certificación de buceo. Hay alrededor de 12 escuelas de buceo, que van desde principiantes hasta niveles profesionales.</p>
    </Section>
</template>