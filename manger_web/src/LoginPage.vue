<template>
    <div>
        <LoginForm></LoginForm>
    </div>
</template>

<script>
    import LoginForm from "./components/login/login_form.vue"
    export default {
        components: {
            LoginForm
        },
        data() {
            return {
                imgSrc: require('./assets/images/back.jpg'),
                username: "",
                password: ""
            }
        }
    }
</script>