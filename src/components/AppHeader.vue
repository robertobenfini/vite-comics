<script>

export default{
    data() {
        return {
            links:[
                {
                    label: 'CHARACTERS',
                    link: '#',
                    active: false
                },
                {
                    label: 'COMICS',
                    link: '#',
                    active: false
                },
                {
                    label: 'MOVIES',
                    link: '#',
                    active: false
                },
                {
                    label: 'TV',
                    link: '#',
                    active: false
                },
                {
                    label: 'GAMES',
                    link: '#',
                    active: false
                },
                {
                    label: 'COLLECTIBLES',
                    link: '#',
                    active: false
                },
                {
                    label: 'VIDEOS',
                    link: '#',
                    active: false
                },
                {
                    label: 'FANS',
                    link: '#',
                    active: false
                },
                {
                    label: 'NEWS',
                    link: '#',
                    active: false
                },
                {
                    label: 'SHOP',
                    link: '#',
                    active: false
                }
            ]
        }
    },
}

</script>

<template>

    <header>
        <div class="container">
            <div class="row">
                <img src="../../public/dc-logo.png" alt="logo">
                <ul>
                    <li v-for="(link, index) in links" :key="index">
                        <a :href="link.link">{{ link.label }}</a>
                    </li>
                </ul>
            </div>
        </div>
    </header>

</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use '../styles/partials/mixins' as *;
    .row{
        @include flex_between;
        
        img{
            width: 75px;
            margin: 15px 0;
        }
        
        ul{
            display: flex;
    
            li{
                height: 100%;
                @include flex_center;
                border: 4px solid transparent;
                
                &:hover{
                    border-bottom: 4px solid $color_blu;
                }

                &:hover a{
                    color:$color_blu;
                }

            
                a{
                    color: black;
                    cursor: pointer;
                    margin: 10px;
                    font-weight: 600;
                    font-size: 12px;
                    
                }
            }
        }
    }

</style>