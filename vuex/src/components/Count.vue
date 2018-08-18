<template>
    <div>
        {{msg}}
        <hr/>
        <h3>{{$store.state.count}}</h3>
        <div>
             <button @click="$store.commit('add')">+</button>
             <button @click="$store.commit('reduce')">-</button>
        </div>
    </div>
   
</template>
<script>
import store from "@/vuex/store"
export default {
    data (){
        return {
            msg:'Hello Vuex'
        }
    },
    store

}
</script>
<style scoped>

</style>
