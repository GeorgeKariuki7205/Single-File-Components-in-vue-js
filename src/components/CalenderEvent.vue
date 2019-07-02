<template>
    <div>
        <p class="card-text" style="background-color:#b77d7d;"><strong>{{ day.abbTitle}}{{events.details}}</strong><span><a href = "#" data-toggle="modal" data-target="#modal" style="margin-right:10%;"><i class="fa fa-trash" style="color:rgb(0,0,10);padding-right:0;"></i></a></span><span><a href="#" data-target = "#modal" data-toggle = "modal"><i class="fa fa-edit" style="color:rgb(0,0,0);"></i></a></span></p>
        <div role="dialog" tabindex="-1" class="modal fade" id = "modal">
    <div class="modal-dialog" role="document">
        <div class="modal-content">
            <div class="modal-header">
                <h4 class="modal-title">Modal Title</h4><button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">×</span></button></div>
            <div class="modal-body">
                <p>The content of your modal.</p>
            </div>
            <div class="modal-footer"><button class="btn btn-light" type="button" data-dismiss="modal">Close</button><button class="btn btn-primary" type="button">Save</button></div>
        </div>
    </div>
</div>
    </div>
</template>
<script>
export default {
    name: 'CalenderEvent',
    props: ['day','events'],
}
</script>
<style lang="scss">

</style>
