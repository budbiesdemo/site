<template>
  <header-view @toggle="toggle"></header-view>
  <sign-in v-if="component === 'signIn'" @toggle="toggle"></sign-in>
  <sign-up v-if="component === 'signUp'" @toggle="toggle"></sign-up>
  <forgot-password v-if="component === 'forgotPassword'" @toggle="toggle"></forgot-password>
  <resetOTP v-if="component === 'resetOTP'" @toggle="toggle"></resetOTP>
  <verify-account v-if="component === 'verifyAccount'" @toggle="toggle"></verify-account>
  <new-password v-if="component === 'newPassword'" @toggle="toggle"></new-password>
  <my-bag v-if="component === 'myBag'" @toggle="toggle"></my-bag>
  <my-address v-if="component === 'user'" @toggle="toggle"></my-address>
  <my-payment v-if="component === 'user'" @toggle="toggle"></my-payment>
  <product-page v-if="component === 'user'" @toggle="toggle"></product-page>
  <wish-list v-if="component === 'wishList'" @toggle="toggle"></wish-list>
</template>

<script>
import HeaderView from './components/headerView.vue'
import SignIn from './components/signIn.vue'
import SignUp from './components/signUp.vue'
import ForgotPassword from './components/forgotPassword.vue'
import ResetOTP from './components/resetOTP.vue'
import VerifyAccount from './components/verifyAccount.vue'
import NewPassword from './components/newPassword.vue'
import MyBag from './components/myBag.vue'
import MyAddress from './components/myAddress.vue'
import MyPayment from './components/myPayment.vue'
import ProductPage from './components/productPage.vue'
import WishList from './components/wishList.vue'

export default {
  name: 'App',
  components: {
    HeaderView,
    SignIn,
    SignUp,
    ForgotPassword,
    ResetOTP,
    VerifyAccount,
    NewPassword,
    MyBag,
    MyAddress,
    MyPayment,
    ProductPage,
    WishList
  },
  data(){
    return{
      component:"",
    };
  },
  methods:{
    toggle(value){
      console.log(value);
      this.component = value;
      
    }
  }
}
</script>

<style>
#app {
  margin: 0;
  padding: 0;
}
body{
  font-family: Helvetica, Arial, sans-serif;
  /* background-color: #F7F7F7; */
}
</style>

