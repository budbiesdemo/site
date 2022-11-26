<template>
    <div class="card">
        <div class="logo">
            BUDBIES
        </div>

        <div class="card-items">
            <div class="card-title">
                SIGN IN
            </div>

            <input type="email" class="e-mail input" placeholder="E-mail">
            <input type="password" class="password input" placeholder="Password">
            <button type="submit" class="button">SIGN IN</button>
            <div class="login-option">
                <input type="checkbox" class="checkbox">Remember me
                <div class="forgot-passowrd"><u @click="toggle('forgotPassword')">Forgot password?</u></div>
            </div>
            <div class="sign-up-link">
                <p>Don't have account?<u @click="toggle('signUp')">Sign up</u></p>
            </div>
        </div>
    </div>

</template>
<script>
export default {
    name: 'signIn',

    methods: {
        toggle(value) {
            this.$emit('toggle', value);
        }
    }
}
</script>

<style scoped>
.logo {
    text-align: center;
    font-size: 30px;
    padding: 10px;
}

.card {
    margin: auto;
    width: 520px;
    height: auto;
    border: 1px solid black;
    border-radius: 10px;
    font-size: 16px;
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
}


.card-title {
    font-size: 20px;
    padding: 8px;
}

.card-items {
    margin: auto;
    display: flex;
    flex-direction: column;
    align-items: center;
}



.input {
    width: 300px;
    height: 30px;
    border: 1px solid black;
    border-radius: 5px;
    margin: 16px;
}

.button {
    margin: 16px;
    width: 304px;
    height: 36px;
    color: white;
    font-size: 16px;
    background-color: #0d6efd;
    border: 1px solid black;
    border-radius: 5px;
}

.button:hover {
    background-color: #005ae0;
    cursor: pointer;
}


.login-option {
    margin: 12px;
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
}

u {
    color: #0d6efd;
    cursor: pointer;
}

.checkbox {
    width: 16px;
    height: 16px;
    border: 1px solid black;
    display: flex;
}

.forgot-passowrd {
    margin-left: 28px;
}
</style>