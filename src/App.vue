<template>
  <Mahasiswi @response="showData" mahasiswi="Sri Adinda"> Ini  adalah nilai  slot dari Parent</Mahasiswi> <br>
  <Mahasiswi @response="showData" mahasiswi="Indri Reynanti"> </Mahasiswi> <br>
  <Mahasiswi @response="showData" mahasiswi="Rahma fatharani"> </Mahasiswi> 

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