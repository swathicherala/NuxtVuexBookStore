<template>
    <div>
       <NuxtLink to="/products">Go Back</NuxtLink>
       <h1>MyItems</h1>
       <!-- {{myRentals}} -->
       <MyItem
       v-for="myrent in myRentals"
       :key="myrent.id"
       :item="myrent"
       />
    </div>
</template>

<script>
import {mapState} from 'vuex'
    export default {
        layout:"no-nav",
        computed:{
           ...mapState([
            'myRentals'
           ])
        }
    }
</script>

<style scoped>

</style>