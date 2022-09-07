<template>
  <div>
      <Nav/>
  <div class="container">
    <Books/>
    <LargeCardDisplay
    v-for="cardInfo in largeCardInfo" 
    :key="cardInfo.id" 
    :cardsSection="cardInfo"
    />
    <SmallCardDisplay
    v-for="smallCard in smallCardInfo"
    :key="smallCard.id"
    :smallCards="smallCard"
    />
  </div>
  </div>
</template>

<script>
import { largeCardSections,smallCardSections } from '../assets/data.js'
export default {
  name: 'IndexPage',
  data(){
    return{
      largeCardInfo:largeCardSections,
      smallCardInfo:smallCardSections
    }
  }
}
</script>
