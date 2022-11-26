<template>
    <div class="card">
        <div class="logo">
            BUDBIES
        </div>

        <div class="card-items">
            <div class="card-title">
                SIGN UP
            </div>
            <div class="user">
                <input type="text" class="name" placeholder="First name">
                <input type="text" class="name" placeholder="Last name">
            </div>
            <input type="number" class="number input" placeholder="Mobile number">
            <input type="email" class="e-mail input" placeholder="E-mail">
            <input type="password" class="password input" placeholder="Password">
            <input type="password" class="password input" placeholder="Confirm password">
            <button type="submit" class="button" @click="toggle('verifyAccount')">SIGN UP</button>
            <div class="signup-option">
                <input type="checkbox" class="checkbox">I agree with terms and conditions.
            </div>
            <div class="sign-up-link">
                <p>Already have account?<u @click="toggle('signIn')">Sign in</u></p>
            </div>
        </div>
    </div>

</template>
<script>
export default {
    name: 'signUp',

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

.user {
    margin: auto;
    display: flex;

}

.name {
    width: 145px;
    height: 30px;
    border: 1px solid black;
    border-radius: 5px;
    margin: 16px 4px;
}

.input {
    width: 300px;
    height: 30px;
    border: 1px solid black;
    border-radius: 5px;
    margin: 16px;
}

input::-webkit-outer-spin-button,
input::-webkit-inner-spin-button {
    -webkit-appearance: none;
    margin: 0;
}

input[type=number] {
    -moz-appearance: textfield;
}


.button {
    margin: 16px;
    width: 305px;
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

.signup-option {
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