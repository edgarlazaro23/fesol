<template lang="pug">
b-container
    b-row
        b-col(sm='6')
            b-row
                b-col(sm='12')
                    <font-awesome-icon icon="mobile-alt"/> 978949562
                b-col(sm='12')
                    <font-awesome-icon icon="mobile-alt"/> 975434851
                b-col(sm='12')
                    <font-awesome-icon icon="envelope"/> fesolinversiones@gmail.com
        b-col(sm='6')
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

            b-button.mt-3(variant="success") Enviar
                
                    
</template>
<script>
export default {
    name: 'Footer',
    data() {
      return {
        nombre: '',
        email: '',
        asunto: '',
        text: ''
      }
    }
}
</script>