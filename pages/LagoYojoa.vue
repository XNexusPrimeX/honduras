<script lang="ts">
import Vue from 'vue';
import Section from '../components/Section.vue';

export default Vue.extend({
    name: 'Lago Yojoa',
    components: {
        Section
    },
    data: () => ({
        image: 'lagoyojoa.jpg',
        author: {
            name: 'Nícolas Estevão Lima',
            pic: 'https://pps.whatsapp.net/v/t61.24694-24/295945714_470306308349840_948209568626474407_n.jpg?ccb=11-4&oh=01_AVyiDJhN7HsvyqCOUj6spw3j_gJ4p1ZarYoZkoXbQGs31w&oe=63435B34'
        }
    })
})
</script>

<template>
    <Section :image="image" :author="author" >
        <p>El lago de Yojoa es la mayor reserva de agua dulce de Honduras, se formó por la explosión de un volcán.</p>
        <p>Yojoa es conocida por su biodiversidad, una gran variedad de aves y plantas, con cerca de 400 especies de aves y 800 especies de plantas identificadas. Desafortunadamente en los últimos años, el lugar ha sufrido por la deforestación.</p>
        <p>Los restaurantes cercanos suelen servir un plato principal, pescado frito “del lago” con rodajas de plátano y pepinillos.</p>
        <p>El lago es un lugar ideal para actividades de ecoturismo, paseos en bote, deportes acuáticos como jet ski, regatas, kayak y pesca.</p>
    </Section>
</template>