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
            pic: 'https://pps.whatsapp.net/v/t61.24694-24/298042111_1035183623866324_7820696349568806522_n.jpg?ccb=11-4&oh=01_AVxsEh-5Q-od2qkRLwp6k5hc26U_rb54WNd2Y5bbWLCdQw&oe=6319B90C'
        }
    })
})
</script>

<template>
    <Section :image="image" :author="author" >
        <p>Las islas son un Área Marina Protegida y están gestionadas por la Fundación Arrecife de Coral de Honduras.</p>
        <p>El arrecife de coral aquí forma parte del segundo sistema de arrecifes de coral más grande del mundo conocido como la Barrera de Coral Mesoamericana.</p>
        <p>Hay una estación de investigación científica en Cayo Menor, la más pequeña de las dos islas principales del sistema.</p>
        <br>
        <p>National Geographic escribe: "Las aguas alrededor de esta colección de cayos de coral son el sueño de un biólogo marino: protegidas por el gobierno, prohibidas para buceadores comerciales y pescadores, y ocupadas con criaturas que aún no tengan nombres"</p>
    </Section>
</template>