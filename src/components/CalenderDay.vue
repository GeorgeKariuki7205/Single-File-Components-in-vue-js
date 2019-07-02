<template>
                    <div class="col-3">
                <div class="card">
                    <div class="card-header" style="background-color:#54cf59;">
                        <h5 class="mb-0">{{day.fullTitle}}</h5>
                    </div>
                    <div class="card-body">
                        <calenderEvent v-for= "(events, index) in day.events" :key="index" :events="events" :day="day"/>
                    </div>
                </div>                
            </div>
</template>


<script>
import CalenderEvent from './CalenderEvent.vue'
export default {
    name: 'CalenderDay',
    props: ['day'],
    components:{
        CalenderEvent
    }
}
</script>


<style lang="scss">

</style>
