<template>
    <div class="container">
        <div class="left-container">
            <div class="left-card">
                <div class="payment-method"><b>Choose Payment Method</b></div>
                <div class="hr-top"></div>
                <div class="payment-card"></div>
            </div>
        </div>
        <div class="right-container">
            <div class="right-card">
                <h4>Price details (1 item)</h4>
                <div class="hr-top"></div>
                <div class="price-table">
                    <div class="mrp">
                        <h5>Total MRP</h5>
                        <h5>12</h5>
                    </div>
                    <div class="discount">
                        <h5>Discount on MRP</h5>
                        <h5>8</h5>
                    </div>
                    <div class="shipping">
                        <h5>Shipping Fee</h5>
                        <h5>5</h5>
                    </div>
                    <div class="coupon-code">
                        <h5>Coupon code</h5>
                        <h5>12</h5>
                    </div>
                    <h5 class="c-code">FIRST005</h5>
                </div>
                <div class="hr-bottom"></div>
                <div class="price-total">
                    <h5><b>Total (MRP)</b></h5>
                    <h5><b>20</b></h5>
                </div>
            </div>
        </div>
    </div>

</template>
<script>
export default {
    name: 'myPayment'

}
</script>

<style scoped>
.container {
    margin: 24px 100px;
    display: flex;
}

@media(max-width: 800px) {
    .container {
        flex-direction: column;
        margin: 0;
    }
}


.left-container {
    display: flex;
    flex-direction: column;
    flex: 1;

}

.left-card {
    display: flex;
    flex-direction: column;
    border: 1px solid black;
    border-radius: 5px;
    margin: 16px;
}


.payment-method {
    margin: 16px 32px;
}

.payment-card {
    margin: 16px 32px;
    height: 100px;
    border: 1px solid black;
    border-radius: 5px;
}



.right-container {
    display: flex;
    flex-direction: column;
    flex: 1;
}




.right-card {
    display: flex;
    flex-direction: column;
    flex: 1;
    border: 1px solid black;
    border-radius: 5px;
    margin: 16px;
}

h4 {
    margin: 16px 32px;
}


.price-table {
    display: flex;
    flex-direction: column;
}

.hr-top {
    border-top: 1px solid gray;
    margin: 0 32px;
    padding-bottom: 12px;
}

h5 {
    margin: 6px 64px;
}


.mrp,
.discount,
.shipping,
.coupon-code,
.price-total {
    display: flex;
    justify-content: space-between;
}


.price-total {
    padding-top: 12px;
    margin-bottom: 16px;
}

b {
    font-size: 16px;
}

.c-code {
    font-size: 16px;
    font-weight: normal;
}



.hr-bottom {
    border-bottom: 1px solid gray;
    margin: 0 64px;
    padding-top: 12px;
}
</style>