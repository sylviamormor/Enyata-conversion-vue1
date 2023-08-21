<script setup>
import TrendcardsComponent from '../TrendcardsComponent.vue';
import facebk from '../assets/facebook.png'
import twit from '../assets/twitter.png'
import pink from '../assets/pink.png'
import pintrest from '../assets/pintrest.png'
import halfblack from '../assets/m-icon.png'
import black from '../assets/m.png'
import orange from '../assets/orange.png'
import vk from '../assets/vk.png'
import linkedin from '../assets/linkedin.png'
</script>

<template>
  
    <div class="firstSet">
<TrendcardsComponent class="tc1" :trend="facebk" />
      <TrendcardsComponent  class="tc2" :trend="twit"/>
      <TrendcardsComponent  class="tc3" :trend="pink"  />
      <TrendcardsComponent  class="tc4" :trend="pintrest"  />
      <TrendcardsComponent  class="tc5" :trend="halfblack"  />
    <TrendcardsComponent class="tc6" :trend="black" />
        <TrendcardsComponent class="tc6" :trend="orange" />
      <TrendcardsComponent  class="tc6" :trend="vk"/>
      <TrendcardsComponent  class="tc6" :trend="linkedin"  />
    </div>
</template>

<style scoped>

.firstSet{
padding-left: 18px;
display: flex;
gap: 18px;
padding-right: 0px;
align-items: center;
justify-content: center;
}

.tc2{

background: #A8FF35;
}
.tc6{
  display: none;
}

@media (min-width: 785px) {

.tc6{
  display: block;
}
.tc5{
  display: none;
}
}

</style>