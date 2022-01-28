<template>
    <header>
        <div class="container">
            <div class="content-logo">
                <img src="../assets/dc-logo.png" alt="">
            </div>

            <nav>
                <ul>
                    <li v-for="(link, index) in links" :key="index">{{ link }}</li>
                    
                </ul>
            </nav>
        </div>  
    </header>
</template>

<script>
export default {
    props: {
        links: Array
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/variables.scss';

header {
    height: 100px;

    .container {
        width: 1200px;
        height: 100px;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;

        .content-logo {
            width: 80px;

            img {
                width: 100%;
            }
        }

        nav {
            line-height: 100px;

            ul {
                list-style: none;
                display: flex;
                align-items: center;
                justify-content: center;

                li {
                    margin-left: 10px;
                    font-size: small;
                    cursor: pointer;

                    &:hover {
                        color: $blue-primary-color;
                        box-shadow: inset 0 -3px 0 $blue-primary-color;
                    }
                }
                
            }
        }

    }



}
</style>