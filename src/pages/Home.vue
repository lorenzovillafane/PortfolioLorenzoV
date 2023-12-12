<template>
  <div>
    <component :is="currentComponent"></component>
  </div>
</template>

<script>
import MenuMobile from '../pages/MenuMobile.vue';
import MenuDesktop from '../pages/MenuDesktop.vue';

export default {
  data() {
    return {
      currentComponent: null,
    };
  },
  mounted() {
    // Llama a la función para establecer el componente inicial al cargar la página
    this.setComponentBasedOnWindowSize();

    // Agrega un event listener para detectar cambios en el tamaño de la ventana
    window.addEventListener('resize', this.setComponentBasedOnWindowSize);
  },
  beforeDestroy() {
    // Elimina el event listener cuando el componente se destruye para evitar problemas de memoria
    window.removeEventListener('resize', this.setComponentBasedOnWindowSize);
  },
  methods: {
    setComponentBasedOnWindowSize() {
      if (window.innerWidth <= 680) {
        this.currentComponent = MenuMobile;
      } else {
        this.currentComponent = MenuDesktop;
      }
    },
  },
  components: {
    MenuMobile,
    MenuDesktop,
  },
};
</script>