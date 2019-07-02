<template>
       <div>         
        <div class="row">
                <CalenderDay v-for= "day in storedData.seedData" :key= "day.id" :day = "day"/>
        </div>
       </div>
</template>
<script>
import {store} from '../store.js'
import CalenderDay from './CalenderDay.vue'
export default {
    name:'CalenderWeek',
    data(){
        return {storedData: store.state}
    },
    components:{
        CalenderDay
    }
}
</script>
<style lang="scss">

</style>
