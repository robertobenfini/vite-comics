<script>
export default {
    data() {
        return {
            links:[
                {
                    icon: './src/assets/buy-comics-digital-comics.png',
                    text: 'DIGITAL COMICS'
                },

                {
                    icon: './src/assets/buy-comics-merchandise.png',
                    text: 'DC MERCHANDISE'
                },

                {
                    icon: './src/assets/buy-comics-subscriptions.png',
                    text: 'SUBSCRIPTION'
                },
                {
                    icon: './src/assets/buy-comics-shop-locator.png',
                    text: 'COMIC SHOP LOCATOR'
                },
                {
                    icon: './src/assets/buy-dc-power-visa.svg',
                    text: 'DC POWER VISA'
                }
            ]
        }
    },
    
}
</script>

<template>
    <div class="container">
        <div class="row">
            <div class="flex" v-for="(link, index) in links" :key="index">
                <img :src="link.icon">
                <div>{{ link.text }}</div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use '../styles/partials/mixins' as *;
.container{
    background-color: $color_blu;
    color: white;
    display: flex;

    .row{
        
        @include flex_center;
        padding: 35px 0;

        .flex{
            @include flex_center;
        }
        img{
            width: 30%;
            margin-left: 40px;
        }

        div{
            margin-left: 10px;
            font-size: 12px;
        }

    }
}
</style>