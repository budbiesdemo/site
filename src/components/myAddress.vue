<template>
    <div class="container">
        <div class="left-container">
            <div class="left-top-card">
                <div class="address"><b>Select delivery address</b></div>
                <button type="submit" class="address-button">ADD NEW ADDRESS</button>
            </div>
            <div class="left-center-card">
                <div class="all-addresses">ADDRESSES</div>
                <div class="hr-top"></div>
                <div class="home-default">
                    <div class="radio"></div>
                    <div class="address-person-name">Ankit Maurya</div>
                    <div class="address-type">HOME</div>
                </div>
                <div class="person-address">Hey this my address and i live here</div>
                <div class="person-contact-details">
                    <div class="mobile-title">Mobile :</div>
                    <div class="person-mobile-number">8850564320</div>
                </div>
                <div class="delivery-type">
                    <div class="status-dot"></div>
                    <div class="delivery-type-status">Pay on delivery is not availabale</div>
                </div>
                <div class="address-modify">
                    <button type="submit" class="remove-button">REMOVE</button>
                    <button type="submit" class="edit-button">EDIT</button>
                </div>
            </div>
            <div class="left-bottom-card">
                <div class="plus-icon">+</div>
                <div class="add-address">Add new address</div>
            </div>
        </div>
        <div class="right-container">
            <div class="right-top-card">
                <div class="estimate-title">Delivery Estimates</div>
                <div class="thumbnail-details">
                    <div class="item-thumbnail"></div>
                    <div class="item-estimate">Estimated delivery by <b>tomorrow</b></div>
                </div>
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
                <button type="button" class="continue-button">CONTINUE</button>
            </div>
        </div>
    </div>

</template>
<script>
export default {
    name: 'myAddress'

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
    background-color: white;
    border: 1px solid black;
    border-radius: 5px;
    width: 180px;
    height: 42px;
    margin: 16px 32px 16px 0;
}


.address-button:hover {
    background-color: black;
    color: white;
    cursor: pointer;
}

.left-center-card {
    display: flex;
    flex-direction: column;
    margin: 16px;
    border: 1px solid black;
    border-radius: 5px;
}

.all-addresses {
    padding: 16px 0;
    margin-left: 32px;
    font-size: 16px;
}

.home-default {
    display: flex;
    align-items: center;
    margin: 0 32px;
}

.radio {
    width: 8px;
    height: 8px;
    margin: 0;
    border: 4px solid blue;
    border-radius: 50%;
}


.address-person-name {
    margin: 0 16px;
    font-weight: bold;
}

.address-type {
    display: flex;
    border: 1px solid darkgreen;
    border-radius: 15px;
    background-color: green;
    color: white;
    padding: 6px;
    font-size: 10px;
    text-align: center;
}



.person-address {
    margin: 16px 64px;
}

.person-contact-details {
    display: flex;
    align-items: center;
    margin: 0 64px;
}

.person-mobile-number {
    margin: 0 4px;
    font-weight: 600;
}

.delivery-type {
    display: flex;
    align-items: center;
    margin: 32px 64px;
}

.status-dot {
    width: 5px;
    height: 5px;
    background-color: black;
    border: 1px solid black;
    border-radius: 5px;
}

.delivery-type-status {
    margin: 0 16px;
}

.address-modify {
    display: flex;
    align-items: center;
    margin: 0 64px 32px 64px;
}

.remove-button {
    width: 100px;
    height: 42px;
    background-color: white;
    border: 1px solid black;
    border-radius: 5px;
}

.edit-button {
    width: 100px;
    height: 42px;
    margin: 0 32px;
    background-color: white;
    border: 1px solid black;
    border-radius: 5px;
}

.remove-button:hover,
.edit-button:hover {
    background-color: black;
    color: white;
    cursor: pointer;
}


.left-bottom-card {
    display: flex;
    align-items: center;
    border: 1px solid black;
    border-radius: 5px;
    margin: 16px;
}

.plus-icon {
    margin: 16px 0px 16px 64px;
    color: red;
}

.add-address {
    margin-left: 8px;
    text-decoration: underline;
    color: red;
}

.add-address:hover {
    cursor: pointer;
}



.right-container {
    display: flex;
    flex-direction: column;
    flex: 1;
}


.right-top-card {
    border: 1px solid black;
    border-radius: 5px;
    margin: 16px;
}

.estimate-title{
    margin: 16px 0px 0px 64px;
}
.thumbnail-details{
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin: 16px 64px;
}


.item-thumbnail{
    width: 104px;
    height: 104px;
    border: 1px solid black;
    border-radius: 5px;
}

.item-estimate{
    margin-right: 64px;
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

.continue-button {
    font-size: 16px;
    height: 42px;
    margin: 32px 64px;
    color: white;
    background-color: orangered;
    border: none;
    border-radius: 5px;
}

.continue-button:hover {
    background-color: red;
    cursor: pointer;
}
</style>