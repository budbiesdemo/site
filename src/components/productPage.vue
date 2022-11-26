<template>
    <div class="container">
        <div class="left-container">
        </div>
        <div class="right-container">
            <div class="product product-title">Budbies Shoes</div>
            <div class="product product-sub-title">Men's running shoes</div>
            <div class="product product-price"> &#8377; 2,999 </div>
            <div class="product product-rating"></div>
            <div class="product product-details">Lorem ipsum dolor sit amet.</div>
            <div class="product product-option">
                <div class="product-option-colors">
                    <div class="product-color-black"></div>
                    <div class="product-color-white"></div>
                    <div class="product-color-blue"></div>
                    <div class="product-color-red"></div>
                    <div class="product-color-yellow"></div>
                </div>
                <div class="product-option-sizes">7 8 9 10</div>
            </div>
            <div class="product product-select-quantity">select quantity</div>
            <div class="product product-availability">Available in stock</div>
            <div class="product product-option-button">
                <button type="button" class="product-add-bag">ADD TO BAG</button>
                <button type="button" class="product-wishlist">WISHLIST</button>
                <button type="button" class="product-buy-now">BUY NOW</button>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'productPage'

}
</script>

<style scoped>
.container {
    display: flex;
    justify-content: center;
    margin: 100px;
    height: 500px;
}

.left-container {
    display: flex;
    flex-direction: column;
    flex: 1;
    border: 1px solid black;
    border-right: none;
    border-top-left-radius: 5px;
    border-bottom-left-radius: 5px;
    margin: 16px 0 16px 16px;
    width: auto;
}


.right-container {
    display: flex;
    flex-direction: column;
    flex: 1;
    border: 1px solid black;
    border-left: none;
    border-top-right-radius: 5px;
    border-bottom-right-radius: 5px;
    margin: 16px 16px 16px 0;
}

.product{
    margin: 4px 0 4px 32px;
}


.product-title{
    margin: 32px 0 4px 32px;
    font-size: 24px;
}


.product-sub-title{
    margin: 4product px 0 0 32px;
}

.product-price{
    font-weight: bold;
}

.product-rating{
    width: 200px;
    height: 10px;
    border-radius: 5px;
    background-color: orange;
}


.product-option-button{
    display: flex;
    justify-content: start;
}
.product-add-bag{
    width: 100px;
    height: 40px;
    margin-right: 8px;
    background-color: orange;
    border: none;
    border-radius: 5px;
}
.product-wishlist{
    width: 100px;
    height: 40px;
    margin: 0 8px;
    background-color: aquamarine;
    border: none;
    border-radius: 5px;
}
.product-buy-now{
    width: 100px;
    height: 40px;
    margin-left: 8px;
    background-color: greenyellow;
    border: none;
    border-radius: 5px;
}


.product-add-bag:hover, .product-wishlist:hover, .product-buy-now:hover{
border: 1px solid gray;
}
</style>