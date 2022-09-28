<script lang="ts">
    import Vue from 'vue';
    import Section from '../components/Section.vue';
    
    export default Vue.extend({
        name: 'Tegucigalpa',
        components: {
            Section
        },
        data: () => ({
            image: 'tegucigalpa.jpg',
            author: {
                name: 'Victória',
                pic: 'https://pps.whatsapp.net/v/t61.24694-24/168406743_544606683581203_1355338904669233688_n.jpg?ccb=11-4&oh=01_AVwEN2rt0Mbzuqni0wUJS5B6uNllijbyVf3hU4FNnOkj9A&oe=63457AF1'
            }
        })
    })
</script>
    
<template>
    <Section :image="image" :author="author" >
        <p>Descubierto por Cristóbal Colón en 1502, Honduras es un país centroamericano con una rica historia y una naturaleza exuberante, que va desde ruinas mayas hasta playas paradisíacas bañadas por el Mar Caribe.</p>
        <p>Como está bajo el radar de la mayoría de los turistas que visitan América Central, la región conserva sus características locales bien conservadas, lo que permite a los viajeros "zambullirse" profundamente en una cultura genuinamente diferente.</p>
        <p>La capital de Honduras es la ciudad de Tegucigalpa, ubicada en la región centro-sur del país, a medio camino entre las fronteras con El Salvador y Nicaragua.</p>
    </Section>
</template>