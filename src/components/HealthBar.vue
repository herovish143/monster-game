<template>
    <section class="container">
        <h2>{{ title }}</h2>
        <div class="healthbar">
            <div class="healthbar__value" :style="{ width: healthBar+'%' }" ></div>
        </div>
    </section>
</template>

<script>
export default {
    props: {
        title: String,
        health: Number
    },
    data() {
        return {
            healthBar: this.health
        }
    }

}
</script>

<style>

</style>