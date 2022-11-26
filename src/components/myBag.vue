<template>
    <div class="container">
        <div class="left-container">
            <div class="left-top-card">
                <div class="address">Adress are here</div>
                <button type="submit" class="address-button">CHANGE</button>
            </div>
            <div class="left-center-card">
                <div class="bag-item-quantity">Items</div>
            </div>
            <div class="left-bottom-card">
                <div class="item-image"></div>
                <div class="item-details"></div>
            </div>
        </div>
        <div class="right-container">
            <div class="right-top-card">
                <div class="coupon">
                    <div class="coupon-icon">icon</div>
                    <h3>COUPONS</h3>
                </div>
                <button type="button" class="apply-button">Apply</button>
            </div>
            <div class="right-bottom-card">
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
                <button type="button" class="place-order">PLACE ORDER</button>
            </div>
        </div>
    </div>

</template>
<script>
export default {
    name: 'myBag',
    methods: {
        toggle(value) {
            this.$emit('toggle', value);
        }
    }

}
</script>

<style scoped>
.container {
    margin: 0 100px;
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


.left-top-card {
    display: flex;
    align-items: center;
    justify-content: space-between;
    border: 1px solid black;
    border-radius: 5px;
    margin: 16px;
}


.address {
    margin-left: 32px;
    padding: 16px 0;
}

.address-button {
    background-color: aqua;
    border: none;
    border-radius: 5px;
    width: 100px;
    height: 42px;
    margin: 16px 32px 16px 0;
}


.address-button:hover {
    background-color: #0dcaf0;
    cursor: pointer;
}

.left-center-card {
    display: flex;
    align-items: center;
    margin: 16px;
    border: 1px solid black;
    border-radius: 5px;
}

.bag-item-quantity {
    padding: 16px 0;
    margin-left: 32px;
    font-size: 22px;
}

.left-bottom-card {
    display: flex;
    justify-content: center;
    border: 1px solid black;
    border-radius: 5px;
    margin: 16px;
    height: 100px;
}


.item-image {
    display: flex;
    flex: 1;
    background-color: lightgray;
    border-top-left-radius: 4px;
    border-bottom-left-radius: 4px;
}

.item-details {
    display: flex;
    flex: 1;
}


.right-container {
    display: flex;
    flex-direction: column;
    flex: 1;
}


.right-top-card {
    display: flex;
    align-items: center;
    justify-content: space-between;
    border: 1px solid black;
    border-radius: 5px;
    margin: 16px;
}


.coupon {
    display: flex;
    margin-left: 32px;
}

.coupon-icon {
    display: flex;
    margin-right: 16px;
    align-items: center;
}


.apply-button {
    width: 100px;
    height: 42px;
    border-radius: 5px;
    border: none;
    margin: 16px 32px 16px 0;
    background-color: #ffa600;

}

.apply-button:hover {
    background-color: #fd7e14;
    cursor: pointer;
}



.right-bottom-card {
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
}

hr {
    color: black;
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

.place-order {
    font-size: 16px;
    height: 42px;
    margin: 32px 64px;
    color: white;
    background-color: orangered;
    border: none;
    border-radius: 5px;
}

.place-order:hover {
    background-color: red;
    cursor: pointer;
}
</style>