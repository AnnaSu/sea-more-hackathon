<template>
    <header class="header">
        <img class="header-icon header__setting" src="../assets/icon_setting.svg" alt="">
        <div class="header__location">
            <img class="header-icon" src="../assets/icon_location.svg" alt="">
            <p class="header__location__name">新北市 白沙灣</p>
        </div>
        <img class="header-icon header__pin" src="../assets/icon_pin.svg" alt="">
    </header>  
</template>

<script>
    
</script>

<style lang="scss">
    .header {
        padding: 10px;
        text-align: center;

        .header-icon {
            width: 20px;
            height: 20px;
            display: inline-block;
            vertical-align: bottom;
            cursor: pointer;
        }

        .header__setting {
            position: fixed;
            left: 10px;
        }

        .header__pin {
            position: fixed;
            right: 10px;
        }

        .header__location, .header__location__name {
            display: inline-block;
            cursor: pointer;
            text-align: center;
        }
    }
</style>
