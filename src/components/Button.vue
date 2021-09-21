<template>
    <button @click="$emit('btn-click')"> {{operator}} </button>
</template>

<script>
export default {
    name: 'Button',
    props: {
        operator: String
    }
}
</script>