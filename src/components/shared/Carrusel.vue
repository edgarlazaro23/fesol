<template lang="pug">
	b-carousel#carousel-1(v-model='slide', :interval='4000', controls='', indicators='' background='#ababab', style='text-shadow: 1px 1px 2px #333;', @sliding-start='onSlideStart', @sliding-end='onSlideEnd')
		div(v-for="(item, i) in imagenes", :key="i" )
			b-carousel-slide(:img-src="item.src", :caption="item.titulo", :text='item.text')
</template>
<script>
import imagenOne  from "../../assets/img/carrusel/1.png";
import imagenTwo  from "../../assets/img/carrusel/2.png";
import imagenTree from "../../assets/img/carrusel/3.png";
import imagenFour  from "../../assets/img/carrusel/4.png";
	export default {
		data() {
			return {
				imagenes:[
					{ src: imagenTwo, titulo: 'IMAGEN 1', text:'Primera imagen de prueba' },
					{ src: imagenOne, titulo: 'IMAGEN 2', text:'Primera imagen de prueba' },
					{ src: imagenTree, titulo: 'CAMARA DE ALMACENAMIENTO (LURÍN)', text:'Primera imagen de prueba' },
					{ src: imagenFour, titulo: 'DHL', text:'Primera imagen de prueba' },
				],
					slide: 0,
					sliding: null
				}
			},
			methods: {
				onSlideStart() {
					this.sliding = true
				},
				onSlideEnd() {
					this.sliding = false
				}
		}
	}
</script>
<style lang="scss">

</style>