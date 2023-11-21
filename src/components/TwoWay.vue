<template>
    <div>
        <p>First Name:{{ firstName }}</p>
        <input type="text" v-model.lazy="firstName">
        <p>Last Name:{{ lastName }}</p>
        <input type="text" v-model="lastName">
    </div>
</template>

<script>
export default {
    name: 'TwoWay',
    data() {
        return {
            firstName: "",
            lastName:""
        }
    },
    // methods: {
    //     getInput() {
    //         this.name = event.target.value
    //     }
    // },
}
</script>