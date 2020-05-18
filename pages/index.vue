<template>
  <div class="page bg-white h-full overflow-hidden">
    <header class="header flex">
      <div class="header-menu flex w-350 items-center">
        <img class="h-52 w-114 " src="../static/logo.svg" alt="User picture">
        <div class="header-circle rounded-full flex items-center justify-center">
          <img class="h-52 w-114" src="../static/menu-outline.svg" alt="User picture">
        </div>
      </div>
      <div class="header-nav flex items-center">
        <div class="header-icon flex w-200">
          <img class="h-6 w-6 " src="../static/help-circle-outline.svg" alt="User picture">
          <img class="h-6 w-6 " src="../static/cart-outline.svg" alt="User picture">
          <img class="h-6 w-6 " src="../static/notifications-outline.svg" alt="User picture">
        </div>
        <div class="max-w-sm flex  items-center  p-6 rounded-lg user-block">
          <div class="flex-shrink-0">
            <img class="h-12 w-12" src="../static/image.svg" alt="ChitChat Logo">
          </div>
          <div class="ml-6 pt-1 text-center flex">
            <h4 class="text-xl leading-tight text-white px-4">Nick Rough</h4>
            <img class="h-6 w-3" src="../static/arrow.svg" alt="User picture">
          </div>
        </div>
      </div>
    </header>

    <main class="main flex h-full">
      <div class="AppNav flex pl-16 flex-col">
        <div class="nav_item flex items-center">
          <img class="h-5 w-5 mr-4" src="../static/nav_i_1.svg" alt="Item_1">
          <div class="my-8">Dashboard</div>
        </div>
        <div class="nav_item  flex items-center">
          <img class="h-5 w-5 mr-4" src="../static/nav_i_2.svg" alt="Item_2">
          <div class="my-8">My Projects</div>
        </div>
        <div class="nav_item  flex items-center">
          <img class="h-5 w-5 mr-4" src="../static/nav_i_3.svg" alt="Item_3">
          <div class="my-8">News Feed</div>
        </div>
        <div class="nav_item  flex items-center">
          <img class="h-5 w-5 mr-4" src="../static/nav_i_4.svg" alt="Item_4">
          <div class="my-8">My Notes</div>
        </div>
        <div class="nav_item  flex items-center">
          <img class="h-5 w-5 mr-4" src="../static/nav_i_5.svg" alt="Item_5">
          <div class="my-8">Messages</div>
        </div>
        <div class="nav_item  flex items-center">
          <img class="h-5 w-5 mr-4" src="../static/nav_i_6.svg" alt="Item_6">
          <div class="my-8">Blog</div>
        </div>
      </div>

      <div class="AppPage w-screen h-full">
        <div class="flex items-center justify-start flex-col bg-white Shadow h-full">
          <div class="OrderSteps m-12 flex justify-center items-start pt-8 relative">
            <div class="Step1 mx-6 flex items-center flex-col justify-center relative z-10">
              <div class="bg-black flex items-center justify-center rounded-full w-16 h-16">
                <img class="h-6 w-6" src="../static/steps_i_1.svg" alt="Item_1">
              </div>
              <div class="pt-5 text-xl">Overview</div>
            </div>

            <div class="Step2 mx-6 flex items-center flex-col justify-center relative z-10">
              <div class="bg-black flex items-center justify-center rounded-full w-16 h-16">
                <img class="h-6 w-6" src="../static/steps_i_2.svg" alt="Item_2">
              </div>
              <div class="pt-5 text-xl">Cart</div>
            </div>

            <div class="Step3 mx-6 flex items-center flex-col justify-center relative z-10">
              <div class="bg-black flex items-center justify-center rounded-full w-16 h-16">
                <img class="h-6 w-6" src="../static/steps_i_3.svg" alt="Item_3">
              </div>
              <div class="pt-5 text-xl">Add Service</div>
            </div>

            <div class="Step4 mx-6 flex items-center flex-col justify-center relative z-10">
              <div class="bg-black flex items-center justify-center rounded-full w-16 h-16">
                <img class="h-6 w-6" src="../static/steps_i_4.svg" alt="Item_4">
              </div>
              <div class="pt-5 text-xl">Delivery</div>
            </div>

            <div class="Step5 mx-6 flex items-center flex-col justify-center relative z-10">
              <div class="bg-black flex items-center justify-center rounded-full w-16 h-16">
                <img class="h-6 w-6" src="../static/steps_i_5.svg" alt="Item_5">
              </div>
              <div class="pt-5 text-xl">Payment</div>
            </div>

            <div class="Step6 mx-6 flex items-center flex-col justify-center relative z-10">
              <div class="bg-pink-500 flex items-center justify-center rounded-full w-16 h-16">
                <img class="h-6 w-6" src="../static/steps_i_6.svg" alt="Item_6">
              </div>
              <div class="pt-5 text-xl text-pink-500">Confirmation</div>
            </div>

            <div class="black-line h-14 absolute bg-black w-20"></div>
          </div>
          <div class="congratulation flex items-center flex-col justify-center">
            <img class="h-32 w-32" src="../static/present.svg" alt="User picture">
            <div class="flex flex-col items-center my-4">
              <p class="pt-5 text-4xl text-pink-500">Congratulations!</p>
              <p class="text-black text-4xl">You order is accepted.</p>
            </div>
            <button class="bg-pink-500 text-white hover:bg-pink-700 font-bold py-2 px-4 rounded flex items-center justify-center">
              Track order
              <img class="h-6 w-3" src="../static/arrow-right.svg" alt="User picture">
            </button>
          </div>
        </div>
      </div>
    </main>



  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style>
.header {
  height: 120px;
  justify-content: space-between;
}
.header-nav {
  background-image: url("../static/bg.png");
  width: 60vw;
  height: 120px;
  display: block;
  background-position: cover;
  background-repeat: no-repeat;

  display: flex;
  justify-content: flex-end;
}
.header-icon {
  width: 200px;
    justify-content: space-evenly;
}
.header-menu {
  justify-content: space-around;
  width: 350px;
}
.header-circle {
  width: 50px;
  height: 50px;
  border: 1px solid #efefef;

      /* display: flex;
    align-items: center;
    justify-content: center; */
}
.user-block {
  margin:0px;
}
.AppNav {
  /* flex-direction: column; */
    width: 350px;
}
.nav_item {
  font-size: 20px;
  font-size: 20px;
  justify-content: flex-start;
}
.AppPage {
  background-color: rgba(0,0,0,0.05);
      padding: 50px;

}
.OrderSteps {
  height: 150px;
  width: 650px;
}
.Shadow {
  -webkit-box-shadow: 0px 5px 58px 0px rgba(0,0,0,0.5);
-moz-box-shadow: 0px 5px 58px 0px rgba(0,0,0,0.5);
box-shadow: 0px 5px 58px 0px rgba(0,0,0,0.5);
}
.black-line {
  height: 13px;
      width: 100%;
  top: 55px;

}
.congratulation {
  width: 400px;
  height: 400px;
}

</style>