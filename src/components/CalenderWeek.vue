<template>
       <div>         
        <div class="row">
                <CalenderDay />
        </div>
       </div>
</template>
<script>
import CalenderDay from './CalenderDay.vue'
export default {
    name:'CalenderWeek',
    components:{
        CalenderDay
    }
}
</script>
<style lang="scss">

</style>
