<template>
<Mahasiswi @response="(whatever) => seelectedMahasiswi=whatever" mahasiswi="Sri Adinda" /> <br>
<Mahasiswi @response="(whatever) => seelectedMahasiswi=whatever" mahasiswi="Indri Reynanti" /> <br>
<Mahasiswi @response="(whatever) => seelectedMahasiswi=whatever" mahasiswi="Rahma fatharani" /> 
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
    }
  } 
</script>