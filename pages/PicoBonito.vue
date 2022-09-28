<script lang="ts">
import Vue from 'vue';
import Section from '../components/Section.vue';

export default Vue.extend({
    name: 'Pico Bonito',
    components: {
        Section
    },
    data: () => ({
        image: 'picobonito.jpg',
        author: {
            name: 'Nathan Vieira',
            pic: 'https://pps.whatsapp.net/v/t61.24694-24/301365739_484450663116988_2882552638713455696_n.jpg?ccb=11-4&oh=01_AVxD5RZKKPEcIjzf2rfRdUjnwwy8QkJSLUwQ-b_Du6t34A&oe=6344ADF5'
        }
    })
})
</script>

<template>
    <Section :image="image" :author="author" >
        <p>Pico Bonito es un parque nacional en Honduras, se encuentra en la cordillera conocida como Nobre de Dios. El parque fue nombrado en honor al alto pico en su territorio.</p>
 
        <p>Pico Bonito es el segundo parque nacional más grande de Honduras.  Hay bosques nublados y tropicales, una gran cantidad de ríos y dos picos de alta montaña: Pico de Bonito y Montein Corazal.</p>
 
        <p>La fauna del parque es muy diversa y en su territorio se pueden observar muchas aves únicas. También en esta área protegida se puede practicar kayak, rafting y senderismo.  Sin embargo, algunas partes del parque están cerradas a los visitantes comunes: solo tienen acceso grupos científicos y escaladores profesionales.</p>
    </Section>
</template>