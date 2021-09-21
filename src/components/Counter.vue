<template>
    <h2>Count: {{count}}</h2>
    <div class="button">
        <Button @btn-click= "increaseCount" operator="Up Count"/>
        <Button @btn-click= "decreaseCount" operator="Down Count"/>
        <Button @btn-click= "resetCount" operator="Reset"/>
    </div>
</template>

<script>
import Button from './Button.vue'

export default {
    name: 'Counter',
    data() {
        return {
            count: 0
        }
    },
    components: {
        Button
    },
    methods: {
        increaseCount(){
            this.count++
        },
        decreaseCount(){
            this.count--
        },
        resetCount(){
            this.count = 0
        }
    }
}
</script>

