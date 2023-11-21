<template>
    <div>
        <p>Full Name:{{ fullName }}</p>
        <p>
            <label for="">firstName: </label>
            <input type="text" v-model="firstName">
        </p>
        <p>
            <label for="">lastName</label>
            <input type="text" v-model="lastName">
        </p>
    </div>
</template>

<script>
export default {
    name: "ComputeView",
    data() {
        return {
            firstName: "",
            lastName: ""
        }
    },
    computed: {
        fullName() {
            console.log('Re-evaluating fullname')
            return this.firstName + " " + this.lastName
        },
    },
    // methods: {
    //     fullName() {
    //         return this.firstName + " " + this.lastName
    //     },
    // },
}
</script>

