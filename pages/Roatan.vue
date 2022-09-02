<script lang="ts">
import Vue from 'vue';
import Section from '../components/Section.vue';

export default Vue.extend({
    name: 'Roatán',
    components: {
        Section
    },
    data: () => ({
        image: 'roatan.jpg',
        author: {
            name: 'Ícaro',
            pic: ''
        }
    })
})
</script>

<template>
    <Section :image="image" :author="author" >
        <p>Roatán es una de las islas de Honduras en la Bahía del Caribe. Es parte de la enorme Barrera de Coral Mesoamericana y es conocida por sus playas, sitios de buceo y vida marina, incluidos los tiburones ballena. Al suroeste se encuentra la bulliciosa playa de West Bay, con un arrecife de coral cerca de la costa. Los cruceros atracan en la capital de Coxen Hole y cerca de Mahogany Bay. Al este hay pueblos más pequeños, incluido el pueblo garífuna de Punta Gorda.</p>
        <p>Superficie: 83 km²</p>
        <p>Ubicación: Mar Caribe</p>
        <p>Elegida en 2015 como la tercera isla más bella del mundo</p>
    </Section>
</template>