<template>
     <div>
         <div class="row" style="margin-top:5%;">
                <div class="col-sm-12 col-md-6 offset-md-3">
                    <div class="card">
                        <div class="card-header" style="background-color:#8ecf88;">
                            <h5 class="mb-0">Add Event...</h5>
                        </div>
                        <div class="card-body">
                            <span>{{titleOfDay}}</span>
                            <form>
                                <div class="form-group"><select class="form-control"><option value="Monday" selected="">Monday</option><option value="Teusday">Teusday</option><option value="Wednesday">Wednesday</option><option value="Thursday">Thursday</option><option value="Friday">Friday</option></select></div>
                                <div
                                    class="form-group">
                                    <div class="input-group">
                                        <div class="input-group-prepend"><span class="input-group-text" style="background-color:rgb(188,203,218);"><i class="fa fa-pencil-square-o" style="font-size:22px;background-color:#ffffff;"></i></span></div><input class="form-control" type="text">
                                        <div
                                            class="input-group-append"><button class="btn btn-primary" type="button">Add.</button></div>
                        </div>
                    </div>
                    </form>
                </div>
            </div>
        </div>
    </div>
    </div>
</template>
<script>
import {store} from '../store.js'
export default {
    name:'CalenderEntry',
    computed: {
        titleOfDay(){
            return store.getActiveDay().fullTitle;
        }
    },
}
</script>
<style lang="scss">
    
</style>