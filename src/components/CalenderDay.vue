<template>
                    <div class="col-sm-5 col-md-4 col-lg-3 col-xl-3 offset-sm-1" style="margin-bottom:7%;cursor:pointer;" @click = "setActiveDay(day.id)">
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
import {store} from '../store.js' 
export default {
    name: 'CalenderDay',
    props: ['day'],
    components:{
        CalenderEvent
    },
    methods: {
        setActiveDay(dayId){
            store.setActiveDay(dayId);
        // document.write(this.day.fullTitle);
 
        }
    },
}
</script>


<style lang="scss">

</style>
