<template>
    <div class="card">
        <div class="logo">
            BUDBIES
        </div>
        <div class="card-items">
            <div class="card-title">
                FORGOT PASSOWRD?
            </div>
            <h5>To reset your password, enter registered E-mail</h5>
            <input type="email" class="e-mail input" placeholder="E-mail">
            <button type="submit" class="button" @click="toggle('resetOTP')">CONTINUE</button>
        </div>
    </div>

</template>
<script>
export default {
    name: 'forgotPassword',

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
</style>