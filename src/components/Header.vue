<template lang="pug">
    b-navbar(toggleable="lg", type="dark",variant="info")
        b-navbar-brand(href='#') NavBar
        b-navbar-toggle(target="nav-collapse")
        b-collapse#nav-collapse(is-nav='')
            b-navbar-nav.ml-auto
                b-nav-item(href="#") Inicio 
                b-nav-item(href="#") Nosotros 
                b-nav-item(href="#") Servicios 
                b-nav-item(href="#") Contactenos 
</template>
<script>
export default {
    name: 'Header'
}
</script>