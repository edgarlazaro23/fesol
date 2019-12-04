<template lang="pug">
.content-page
    b-row
        b-col
            carruselComponent
    b-row
        b-col(sm='3')
            cardComponent
</template>
<script>
import cardComponent from "../components/shared/Card.vue";
import carruselComponent from "../components/shared/Carrusel.vue";

export default {
    name: "Content",
    components: {
        cardComponent,
        carruselComponent
    }
};
</script>