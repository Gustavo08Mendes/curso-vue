<template>
    <div>
        <Avatar />
        <h1>Esta é a descrição da Pessoa: {{ nome }}</h1>
        <Info />
        <Formulario />
    </div>
</template>

<script>
import Formulario from './formulario/input.vue';
import Info from './info.vue';
import Avatar from './Picture.vue';
    export default {
        name: 'Pessoa',
        data() {
            return {
                nome: 'Gustavo',
            }
        },
        components: {
            Info,
            Formulario,
            Avatar
        }
    }
</script>