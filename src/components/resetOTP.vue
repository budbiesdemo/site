<template>
    <div class="card">
        <div class="logo">
            BUDBIES
        </div>
        <div class="card-items">
            <div class="card-title">
                OTP
            </div>
            <h5>Check your E-mail for OTP</h5>
            <div class="otp-input">
                <input type="text" class="otp">
                <input type="text" class="otp">
                <input type="text" class="otp">
                <input type="text" class="otp">
                <input type="text" class="otp">
                <input type="text" class="otp">
            </div>
            <button type="submit" class="button" @click="toggle('newPassword')">VALIDATE</button>
        </div>
    </div>

</template>
<script>
export default {
    name: 'resetOTP',

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

h5 {
    font-weight: lighter;
    margin: 0px;
}

.card-items {
    margin: auto;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.otp-input {
    margin: 6px;
}

.otp {
    width: 38px;
    height: 30px;
    margin: 12px 4px 2px 4px;
    border: 1px solid black;
    border-radius: 5px;
    text-align: center;
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
</style>