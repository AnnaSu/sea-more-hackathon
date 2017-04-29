<template>
    <div class="indicator-container">

            <div v-for="item in indicators" :class="item.className">
                <div class="name">{{ item.name }}</div>
                <img class="icon" :src="item.icon" />
                <div class="value">{{ item.value }}</div>
            </div>

    </div>
</template>

<script>
export default {
  name: 'indicator',
  data () {
    return {
        indicators: [
            {
                className: 'indicator-item rainfall',
                name: '降雨機率',
                icon: '/src/assets/icon_umbrella.svg',
                value: '15%'
            },
            {
                className: 'indicator-item uv',
                name: '紫外線',
                icon: '/src/assets/icon_uv.svg',
                value: '15%'
            },
            {
                className: 'indicator-item temperature-diff',
                name: '溫差',
                icon: '/src/assets/icon_temp.svg',
                value: '11°'
            },
            {
                className: 'indicator-item tidal',
                name: '潮汐',
                icon: '/src/assets/icon_tidal.svg',
                value: '乾潮'
            },
            {
                className: 'indicator-item wave-height',
                name: '浪高',
                icon: '/src/assets/icon_wave.svg',
                value: '0.8m'
            },
            {
                className: 'indicator-item wind',
                name: '風速',
                icon: '/src/assets/icon_wind.svg',
                value: '3.2km/hr'
            }
        ]
    }
  }
}
</script>

<style lang="css">
.indicator-item:nth-child(1) {
  border-radius: 10px 0 0 0;
}
.indicator-item:nth-child(3) {
  border-radius: 0 10px 0 0;
}
.indicator-item:nth-child(4) {
  border-radius: 0 0 0 10px;
  clear: left;
}
.indicator-item:nth-child(6) {
  border-radius: 0 0 10px 0;
  clear: right;
}
.indicator-item {
    color: #485F79;
    width: 100px;
    height: 100px;
    background: rgba(255,255,255,.8);
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
}
.indicator-item > .icon {
    width: 30px;
    height: 30px;
}
</style>
