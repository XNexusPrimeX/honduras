<script lang="ts">
import Vue from 'vue';
import Section from '../components/Section.vue';

export default Vue.extend({
    name: 'Cochinos',
    components: {
        Section
    },
    data: () => ({
        image: 'cochinos.jpg',
        author: {
            name: 'Isabelle Mendes Meza',
            pic: 'https://pps.whatsapp.net/v/t61.24694-24/301422539_1556102654903996_4458326696991109932_n.jpg?ccb=11-4&oh=01_AVyyfBBhOg5X_hSBA5DyV9DmnBTPgH-qgYmL3JxfuTlcvA&oe=6342F1A9'
        }
    })
})
</script>

<template>
    <Section :image="image" :author="author" >
        <p>Las islas son un Área Marina Protegida y están gestionadas por la Fundación Arrecife de Coral de Honduras.</p>
        <p>El arrecife de coral aquí forma parte del segundo sistema de arrecifes de coral más grande del mundo conocido como la Barrera de Coral Mesoamericana.</p>
        <p>Hay una estación de investigación científica en Cayo Menor, la más pequeña de las dos islas principales del sistema.</p>
        <p>National Geographic escribe: "Las aguas alrededor de esta colección de cayos de coral son el sueño de un biólogo marino: protegidas por el gobierno, prohibidas para buceadores comerciales y pescadores, y ocupadas con criaturas que aún no tengan nombres"</p>
    </Section>
</template>