<template>
    <div>
        <h2> Content </h2>
        <Location />
        <Template />
        <Indicator />
        <Suggestion />
        <Ref />
    </div>  
</template>

<script>
    import Location from './Location.vue';
    import Template from './Tempture.vue';
    import Indicator from './Indicator.vue';
    import Suggestion from './Suggestion.vue';
    import Ref from './Ref.vue';
    export default {
        components: {
            Location,
            Template,
            Indicator,
            Suggestion,
            Ref
        }
    }  
</script>

<style lang="css">
    
</style>
