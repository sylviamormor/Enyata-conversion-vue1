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
    </div>
    <div class="secondSet">
        <TrendcardsComponent class="tc1" :trend="facebk" />
      <TrendcardsComponent  class="tc2" :trend="twit"/>
      <TrendcardsComponent  class="tc3" :trend="pink"  />
      <TrendcardsComponent  class="tc4" :trend="pintrest"  />
    <TrendcardsComponent class="tc6" :trend="black" />
        <TrendcardsComponent class="tc7" :trend="orange" />
      <TrendcardsComponent  class="tc8" :trend="vk"/>
      <TrendcardsComponent  class="tc9" :trend="linkedin"  />
    </div>
</template>

<style scoped>
.secondSet{
display: none;
}
.firstSet{
padding-left: 18px;
display: flex;
gap: 18px;
padding-right: 0px;
align-items: center;
}

.tc2{

background: #A8FF35;
}

@media (min-width: 900px) {
.firstSet{
    display: none;
}
.secondSet{
    display: block;
    width: 124px;
height: 124px;
border-radius: 8px;
padding-left: 18px;
display: flex;
padding-right: 0px;
align-items: center;
gap: 24px;
justify-content: start;
padding: 140px ;
}
}

</style>