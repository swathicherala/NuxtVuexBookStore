<template>
    <div>
        <Nav/>
        <div class="container">
       <LargeCardDisplay
       v-for="cardInfo in largeCardsInfo.slice(0,1)"
       :key="cardInfo.id"
       :cardsSection="cardInfo"
       />
       <SmallCardDisplay
       v-for="cardInfo in smallCardsSection"
       :key="cardInfo.id"
       :smallCards="cardInfo"
       />
    </div>
    </div>
</template>

<script>
import {largeCardSections,smallCardSections} from '@/assets/data.js'
    export default {
        data(){
            return{
                largeCardsInfo:largeCardSections,
                smallCardsSection:smallCardSections
            }
        }
    }
</script>

<style scoped>

</style>