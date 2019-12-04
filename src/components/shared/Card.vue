<template lang="pug">
    b-card-group(deck)
        b-card(title="Title" img-src="https://picsum.photos/300/300/?image=41", img-alt="Image", img-top)
            b-card-text This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.
            template(v-slot:footer) 
                small.text-muted Last updated 3 mins ago/small
</template>
<script>
export default {
    name: 'Card',
    data() {
      return {
      }
    }
}
</script>