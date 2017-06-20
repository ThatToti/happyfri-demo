<template>
    <section>
        <header class="top_tips">
            <span class="num_tip" v-if="fatherComponent=='home'">{{level}}</span>
            <span class="num_tip" v-if="fatherComponent=='item'">题目{{itemNum}}</span>
        </header>
    </section>
</template>

<script>
import {mapState,mapActions}from 'vuex'

export default{
    name:'itemcontainer',
    data(){

    },
    computed:mapState({
        itemNum:state=>state.itemNum,
        level:state=>state.level,
        itemDetail:state=>state.itemDetail
    }),
    methods:{
        
    }
}
</script>

<style>
</style>