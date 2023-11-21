<template>
    <div>
        <p>Full Name: {{ fullName }}</p>
        <p><button @click="changeName">Change Name</button></p>
    </div>
</template>

<script>
export default {
    name: "GetterSetter",
    data() {
        return {
            firsName: "Tony",
            lastName:"Stack"
        }
    },
    computed: {
        fullName: {
            get() {
                return this.firsName + " " + this.lastName
            },
            set(value) {
                const names = value.split(' ')
                this.firsName = names[0]
                this.lastName = names[1]
            }
        }
    },
    methods: {
        changeName() {
            this.fullName = 'Iron Man'
        }
    },
}
</script>

<style lang="scss" scoped></style>