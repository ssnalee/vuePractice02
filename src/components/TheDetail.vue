<template>
{{$route.params.id}}
<div class="container mt-4">
    <h5>{{list[$route.params.id].title}}</h5>
    <p>{{list[$route.params.id].date}}</p>
    <p>{{list[$route.params.id].content}}</p>
</div>
</template>
<script>
export default {
    name : "theDetail",
    data(){
        return{

        }
    },
    methods(){

    },
    props : {
        list : Array,
    }
}
</script>
<style>

</style>