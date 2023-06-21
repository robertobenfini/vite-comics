<script>
export default {
    props:{
        myCard: Object
    }
}
</script>
<template lang="">
    <div class="card">
        <img :src="myCard.thumb">
        <span class="text"><h4>{{ myCard.series }}</h4></span>
    </div>
</template>
<style lang="scss" scoped>
    .card{
        
        img{ 
            width: 200px;
            height: 250px;
            padding: 20px;
        }

        h4{
            font-size: 10px;
            margin-left: 20px;
        }
    }
</style>