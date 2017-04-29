<template>
    <div class="temperature">
        <div class="temperature__info">
            <img class="temperature__info__icon" src="../assets/icon_sun.svg" alt="">
            <p class="temperature__info__number">氣溫 32°</p>
        </div>
    </div>
</template>

<script>

</script>

<style lang="scss">
    .temperature {
        margin-top: 50px;
        text-align: center;
    }
    .temperature__info__icon {
        width: 20px;
        height: 20px;
        display: inline-block;
        vertical-align: bottom;
        cursor: pointer;
    }
    .temperature__info, .temperature__info__number {
        display: inline-block;
        cursor: pointer;
        text-align: center;
    }
</style>
