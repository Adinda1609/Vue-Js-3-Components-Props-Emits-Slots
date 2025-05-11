<template>
  <Mahasiswi @response="showData" mahasiswi="Sri Adinda" /> <br>
  <Mahasiswi @response="showData" mahasiswi="Indri Reynanti" /> <br>
  <Mahasiswi @response="showData" mahasiswi="Rahma fatharani" /> 
<p>
  Mahasiswi yang dipilih adalah : {{ seelectedMahasiswi }}  
</p>

</template>

<script>
  import Mahasiswi from './components/Mahasiswi.vue';

  export default {
    components : {
      Mahasiswi
    },
    data() {
      return {
        seelectedMahasiswi : ''
      }
    },
    methods : {
      showData(mahasiswi) {
        this.seelectedMahasiswi = mahasiswi;
      }
    }
  } 
</script>