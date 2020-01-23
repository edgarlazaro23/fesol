<template lang="pug">
.footer
    b-container
        b-row
            b-col(sm='6')
                b-row
                    b-col(sm='12')
                        h2.social-title CONTACTO
                    b-col(sm='12')
                        <i class="fas fa-mobile-alt"></i> 978949562
                    b-col(sm='12')
                        <i class="fas fa-mobile-alt"></i> 975434851
                    b-col(sm='12')
                        <i class="far fa-envelope"></i> fesolinversiones@gmail.com
            b-col.contacto(sm='6')
                b-row
                    b-col(sm='6')
                        b-form-input.mt-3(v-model="nombre", placeholder="Nombre")
                    b-col(sm='6')
                        b-form-input.mt-3(v-model="email", placeholder="Email")
                b-row
                    b-col(sm='12')
                        b-form-input.mt-3(v-model="asunto", placeholder="Asunto")
                    b-col(sm='12')
                        b-form-textarea.mt-3#textarea(v-model='text', placeholder='Enter something...', rows='3', max-rows='6')

                b-button.btn-enviar ENVIAR MENSAJE
    b-row
        b-col.social(sm='12')
            b-row
                b-col(sm='12')
                    h4.social-title SÍGUENOS
                b-col(sm='12')
                    .social-facebook
                        <i class="fab fa-facebook-square"></i>
                    .social-instagram
                        <i class="fab fa-instagram"></i>
    b-row
        b-col.legal
            p Copyright © {{anio}}
                a.hipervinculo(href="https://www.facebook.com/elr28", target="_blank") Edgar Lázaro




</template>
<script>
export default {
    name: 'Footer',
    data() {
      return {
        anio: '',
        nombre: '',
        email: '',
        asunto: '',
        text: ''
      }
    },
    mounted() {
        const fecha = new Date();
        this.anio = fecha.getFullYear();
    }
}
</script>
<style lang="scss">
@import '../assets/scss/components/footer.scss';
</style>
