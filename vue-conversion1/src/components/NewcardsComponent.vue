<script setup>
import SocialComponent from './SocialComponent.vue';
import microsoft from '../assets/microsoft.png'
import allianz from '../assets/allianz.png'
import upwork from '../assets/upwork.png'
import volvo from '../assets/volvo.png'
import grab from '../assets/grab.svg'
import verizon from '../assets/verizon.png'
import coinbase from '../assets/coinbase.png'
import expedia from '../assets/expedia 129.png'
import airtable from '../assets/airtable.png'
import magento from '../assets/magneto.png'
import carrera from '../assets/carrera.png'
import bonanza from '../assets/bonanza.png'
import transfer from '../assets/wetransfer.png'
import suzuki from '../assets/suzuki.png'
import algolia from '../assets/algolia.png'
import heineken  from '../assets/heineken.png'
</script>

<template>
<div class="cds">
    <SocialComponent class="cd1" :social="microsoft" />
      <SocialComponent class="cd2" :social="allianz"/>
      <SocialComponent class="cd3" :social="upwork"  />
      <SocialComponent class="cd4" :social="volvo"  />
      <SocialComponent class="cd5" :social="grab"  />
      <SocialComponent class="cd6" :social="verizon"  />
      <SocialComponent class="cd7" :social="coinbase"  />
      <SocialComponent class="cd8" :social="expedia"  />
      <SocialComponent class="cd9" :social="airtable"  />
      <SocialComponent class="cd10" :social="magento"  />
      <SocialComponent class="cd11" :social="carrera"  />
      <SocialComponent class="cd12" :social="bonanza"  />
      <SocialComponent class="cd13" :social="transfer"  />
      <SocialComponent class="cd14" :social="suzuki"  />
      <SocialComponent class="cd15" :social="algolia"  />
      <SocialComponent class="cd16" :social="heineken"  />
</div>
</template>


<style scoped>
.cds{
 display: grid;
 grid-template-columns: repeat(2, 1fr);
 grid-gap: 10px;
}

@media (min-width: 900px) {
.cds{
 display:grid ;
 grid-template-columns: repeat(4, 1fr);
 grid-gap: 10px;
}


}
</style>