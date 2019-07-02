<template>
    <div>
        <p class="card-text" style="background-color:#b77d7d; margin-bottom:5%;"><strong>{{events.details}}  <span>  </span> </strong><span><a href = "#" data-toggle="modal" data-target="#modal" style="margin-right:10%;"><i class="fa fa-trash" style="color:rgb(0,0,10);padding-right:0;"></i></a></span><span><a href="#" data-target = "#modal" data-toggle = "modal"><i class="fa fa-edit" style="color:rgb(0,0,0);"></i></a></span></p>
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
