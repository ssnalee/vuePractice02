<template>
  <div v-for="(a,i) in list" :key="a">
    <h5>{{list[i].title}}</h5>
    <p>{{list[i].date}}</p>
    <!-- <a @click="$router.push(`detail/${i}`)">디테일</a> -->
    <router-link :to="`detail/${i}`">디테일</router-link>
  </div>


</template>
<script>
export default {
    name : "theList",
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