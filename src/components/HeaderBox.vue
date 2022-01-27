<template>
    <header>
        <div class="container">
            <div class="content-logo">
                <img src="@/assets/dc-logo.png" alt="">
            </div>

            <nav>
                <ul>
                    <li>CHARACTERS</li>
                    <li>COMICS</li>
                    <li>MOVIES</li>
                    <li>TV</li>
                    <li>GAMES</li>
                    <li>COLLECTIBLES</li>
                    <li>VIDEOS</li>
                    <li>FANS</li>
                    <li>NEWS</li>
                    <li>SHOP</li>
                </ul>
            </nav>
        </div>  
    </header>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@import '@/style/variables.scss';

header {
    height: 100px;
    border: 1px solid black;

    .container {
        width: 1000px;
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
            height: 100%;
            line-height: 100px;

            ul {
                list-style: none;
                display: flex;
                align-items: center;
                justify-content: center;

                li {
                    height: 100%;
                    margin-left: 10px;
                    font-size: small;
                    cursor: pointer;

                    &:hover {
                        color: $blue-primary-color;
                        border-bottom: 4px solid $blue-primary-color;
                    }
                }
                
            }
        }

    }



}
</style>