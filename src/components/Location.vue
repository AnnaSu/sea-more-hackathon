<template>
    <div class="location">
        <h1 class="location__city">新北市</h1>
        <h1 class="location__name">白沙灣</h1>
        <img class="location__icon" src="../assets/icon_pin.svg" alt="">
    </div>  
</template>

<script>
    
</script>

<style lang="scss">
    .location {
        text-align: center;
        margin-top: 60px;

        .location__icon {
            width: 30px;
            margin: 5px auto 0;
        }

        .location__city{
            font-size: 20px;
            line-height: 30px;
        }

        .location__name  {
            font-size: 30px;
            line-height: 40px;
        }
    }
</style>
