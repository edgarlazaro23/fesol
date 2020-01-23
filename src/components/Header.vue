<template lang="pug">
    b-navbar.header(toggleable="lg", type="dark")
        b-navbar-brand(href='#')
            img.logo(:src="require(`@/assets/img/fesol.png`)", alt="kitten")
        b-navbar-toggle(target="nav-collapse")
        b-collapse#nav-collapse(is-nav='')
            b-navbar-nav.ml-auto
                b-nav-item(href="#") INICIO
                b-nav-item(href="#") NOSOTROS
                b-nav-item(href="#") SERVICIOS
                b-nav-item(href="#") CONTACTO
</template>

<script>
// import fesolIcon  from "../assets/img/fesol.png";
export default {
    name: 'Header'
}
</script>
<style lang="scss">
@import '../assets/scss/components/header.scss';
</style>
