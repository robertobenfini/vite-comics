<script>
export default {
    data() {
        return {
            navs:[
                {icon: './src/assets/buy-comics-digital-comics.png', text: 'DIGITAL COMICS'},
                {icon: './src/assets/buy-comics-merchandise.png', text: 'DC MERCHANDISE'},
                {icon: './src/assets/buy-comics-subscriptions.png', text: 'SUBSCRIPTION'},
                {icon: './src/assets/buy-comics-shop-locator.png', text: 'COMIC SHOP LOCATOR'},
                {icon: './src/assets/buy-dc-power-visa.svg', text: 'DC POWER VISA'}
            ]
        }
    },
    
}
</script>

<template >
    <div class="container">
        <div class="row">
            <div class="flex" v-for="(nav, index) in navs" :key="index">
                <img  :src="nav.icon">
                <div>{{ nav.text }}</div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.container{
    background-color: #0074E8;
    color: white;
    display: flex;

    .row{
        
        display: flex;
        align-items: center;
        padding: 35px 0;

        .flex{
            display: flex;
            align-items: center;
        }
        img{
            width: 60px;
            height: 70px;
            margin-left: 40px;
        }

        div{
            margin-left: 10px;
            font-size: 12px;
        }

    }
}
</style>