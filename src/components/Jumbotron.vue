<template>
    <div class="jumbotron">
        <div class="container">
            <div class="current-series">
                <p>CURRENT SERIES</p>
            </div>
        </div>

    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@import "@/style/jumbotron.scss";
@import '../style/variables.scss';

    .jumbotron {
        height: 300px;
        border: 1px solid black;
        background-image: $principle-jumbo;
        background-size: cover;

        .container {
            width: 1000px;
            height: 300px;
            margin: 0 auto;
            position: relative;
        
            .current-series {
                width: 150px;
                position: absolute;
                bottom: -15px;
                left: 0;
                
                p {
                    padding: 10px;
                    background-color: $blue-primary-color;
                    color: white;
                }
            }
        }
    }

</style>