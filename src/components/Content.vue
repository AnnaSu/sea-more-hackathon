<template>
    <div>
        <Location />
        <Temperature :pageIndex="this.pageIndex" />
        <Indicator :pageIndex="this.pageIndex"/>
        <Suggestion />
        <Ref />
    </div>
</template>

<script>
    import Location from './Location.vue';
    import Temperature from './Temperature.vue';
    import Indicator from './Indicator.vue';
    import Suggestion from './Suggestion.vue';
    import Ref from './Ref.vue';
    export default {
        props: ['pageIndex'],
        components: {
            Location,
            Temperature,
            Indicator,
            Suggestion,
            Ref
        }
    }
</script>

<style lang="css">

</style>
