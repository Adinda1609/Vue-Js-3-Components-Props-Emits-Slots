<template>
    <slot>
        ini adalah slot default karena parent component tidak memberikan data
    </slot><br>
    Halo, ini adalah siswi bernama {{ mahasiswi }} 🚀 <button @click="showData">Show Detail</button><br>
</template>

<script>
    export default {
        props: {
            mahasiswi : String
        },
        emits: ['response'],
        methods: {
            showData() {
                this.$emit('response', this.mahasiswi)
            }
        }
    }
</script>