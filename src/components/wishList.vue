<template>
    <div class="container">
        <div class="container-header">
            <div class="container-title">My Wishlist</div>
            <div class="wishlist-total-item">5 items</div>
        </div>
        <div class="container-cards">
            <div class="wishlist-card">
                <div class="wishlist-item-image"></div>
                <div class="wishlist-item-delete-button">X</div>
                <div class="wishlist-item-name">Budbies T-shirt</div>
                <div class="wishlist-item-price"> &#8377; 2,999 </div>
                <div class="hr-bottom"></div>
                <div class="wishlist-add-to-bag-button">ADD TO BAG</div>
            </div>
            <div class="wishlist-card">
                <div class="wishlist-item-image"></div>
                <div class="wishlist-item-delete-button">X</div>
                <div class="wishlist-item-name">Budbies T-shirt</div>
                <div class="wishlist-item-price"> &#8377; 2,999 </div>
                <div class="hr-bottom"></div>
                <div class="wishlist-add-to-bag-button">ADD TO BAG</div>
            </div>
            <div class="wishlist-card">
                <div class="wishlist-item-image"></div>
                <div class="wishlist-item-delete-button">X</div>
                <div class="wishlist-item-name">Budbies T-shirt</div>
                <div class="wishlist-item-price"> &#8377; 2,999 </div>
                <div class="hr-bottom"></div>
                <div class="wishlist-add-to-bag-button">ADD TO BAG</div>
            </div>
            <div class="wishlist-card">
                <div class="wishlist-item-image"></div>
                <div class="wishlist-item-delete-button">X</div>
                <div class="wishlist-item-name">Budbies T-shirt</div>
                <div class="wishlist-item-price"> &#8377; 2,999 </div>
                <div class="hr-bottom"></div>
                <div class="wishlist-add-to-bag-button">ADD TO BAG</div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'wishList',

    methods: {
        toggle(value) {
            this.$emit('toggle', value);
        }
    }
}
</script>

<style scoped>
.container {
    display: flex;
    flex-direction: column;
    margin: 0 100px;
}


.container-header {
    display: flex;
    align-items: center;
}

.container-title {
    font-weight: bold;
    font-size: 18px;
    margin: 0 4px 16px 16px;
}

.wishlist-total-item {
    margin: 0 0 16px 4px;
}

.container-cards {
    display: flex;
    justify-content: space-between;
    margin: 16px;

}

.wishlist-card {
    position: relative;
    display: flex;
    flex-direction: column;
    height: 500px;
    width: 275px;
    border: 1px solid black;
    border-radius: 5px;
}

.wishlist-card:hover {
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.2);
}

.wishlist-item-image {
    background-color: aquamarine;
    height: 350px;
    border-top-left-radius: 5px;
    border-top-right-radius: 5px;
    display: flex;
}

.wishlist-item-image:hover {
    cursor: pointer;
}

.wishlist-item-delete-button {
    position: absolute;
    top: 8px;
    right: 8px;
    display: flex;
    justify-content: center;
    align-items: center;
    width: 16px;
    height: 16px;

}

.wishlist-item-delete-button:hover {
    color: red;
    cursor: pointer;
    border-radius: 50px;
}

.wishlist-item-name {
    font-weight: bold;
    display: flex;
    justify-content: center;
    margin: 8px;
}

.wishlist-item-price {
    font-weight: bold;
    display: flex;
    justify-content: center;
    margin: 8px;
    flex: 1;
}


.hr-bottom {
    border-top: 1px solid black;
}

.wishlist-add-to-bag-button {
    padding: 16px;
    display: flex;
    justify-content: center;
    background-color: aqua;
    border-bottom-left-radius: 5px;
    border-bottom-right-radius: 5px;
}

.wishlist-add-to-bag-button:hover {
    cursor: pointer;
}
</style>
