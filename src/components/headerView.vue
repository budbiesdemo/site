<template>
  <div class="container_header">
    <div class="left_header">
      <div class="title">
        <h1>BUDBIES</h1>
      </div>
    </div>
    <div class="center_header">
      <div class="search">
        <input type="text" placeholder="Search...">
      </div>
    </div>
    <div class="right_header">
      <ul class="user_content">
        <li class="user__item" >
          <span class="user" @click="toggle('signIn')"></span>
        </li>
        <li class="user__item">
          <span class="wishlist" @click="toggle('wishList')"></span>
        </li>
        <li class="user__item">
          <span class="bag" @click="toggle('myBag')"></span>
          <span class="badge">1</span>
        </li>
      </ul>
    </div>
  </div>
  <ul class="menu">
    <li class="menu__item">NEW</li>
    <li class="menu__item">Mens</li>
    <li class="menu__item">Womens</li>
    <li class="menu__item">Girls</li>
    <li class="menu__item">Boys</li>
    <li class="menu__item">Sport</li>
    <li class="menu__item">Accessories</li>
    <li class="menu__item">SALE</li>
  </ul>
</template>

<script>


export default {
  name: 'headerView',
  props: {
    msg: String
  },

  methods: {
    toggle(value) {
      this.$emit('toggle', value);
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container_header {
  padding-top: 12px;
  display: flex;
  width: 100%;
  align-items: center;
}

.left_header {
  display: flex;
  justify-content: center;
  width: 350px;
}

h1 {
  margin: 0;
}

.center_header {
  display: flex;
  flex-grow: 1;
  flex-direction: column;
  align-items: center;
}

input {
  width: 500px;
  height: 36px;
  border: 1px solid gray;
  border-radius: 8px;
}

.menu {
  display: flex;
  justify-content: center;
  list-style: none;
  font-size: 18px;
  padding-left: 0;
  margin-bottom: 1px;

}

.menu__item {
  padding: 6px 16px;
  border-bottom: 3px solid transparent;
}

.menu__item:hover {
  border-bottom: 3px solid black;
  cursor: pointer;
}


.right_header {
  width: 350px;
}

.user_content {
  display: flex;
  justify-content: center;
  list-style: none;
  margin: 0;
  padding: 0;
}

.user__item {
  margin: 0 18px;
  position: relative;
}

.user {
  background-image: url(../assets/person-circle.svg);
  height: 28px;
  width: 28px;
  background-repeat: no-repeat;
  background-size: contain;
  display: block;
}

.user:hover{
  cursor: pointer;
}

.wishlist {
  background-image: url(../assets/heart-fill.svg);
  height: 28px;
  width: 28px;
  background-repeat: no-repeat;
  background-size: contain;
  display: block;
}

.wishlist:hover{
  cursor: pointer;
}
.bag {
  background-image: url(../assets/bag-check-fill.svg);
  height: 28px;
  width: 28px;
  background-repeat: no-repeat;
  background-size: contain;
  display: block;
}

.bag:hover{
  cursor: pointer;
}

.badge {
  position: absolute;
  bottom: 15px;
  left: 15px;
  padding: 2px;
  background-color: rgb(201, 0, 0);
  height: 20px;
  width: 20px;
  color: white;
  border-radius: 10px;
  text-align: center;
  font-weight: bold;
}
</style>
