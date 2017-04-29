<template>
    <div class="suggestion">
        <h3 class="suggestion__title">外出建議</h3>
        <ul class="suggestion__lists" v-for="suggestion in suggestions">
            <li class="suggestion__list">
                <div class="suggestion__list__bg">
                    <img class="suggestion__list__icon" :src="suggestion.iconUrl" alt="">
                </div>
            </li>
        </ul>
    </div>  
</template>

<script>

export default {
    data () {
        return {
            suggestions: [
                {   
                    name: '比基尼',
                    iconUrl: './src/assets/icon_bikini.svg'
                }
            ]
        }
    }
}
    
</script>

<style lang="scss">
    .suggestion {
        margin-top: 30px;
        text-align: center;
    }

    .suggestion__title {
        margin-bottom: 20px;
    }

    .suggestion__lists {
        .suggestion__list {

            .suggestion__list__bg {
                width: 40px;
                height: 40px;
                padding: 10px;
                border-radius: 50%;
                background-color: white;
                box-shadow: 1px 1px 20px rgba(20%,20%,40%,0.5);
            }

            .suggestion__list__icon {
                width: 40px;
                height: 40px;
            }
        }
    }
</style>
