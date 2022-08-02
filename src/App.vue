<template>
  <div class="logo-container">
    <img class="logo" src="../images/logo.svg" alt="Bolt Food" />
  </div>
  <div class="dashboard">
    <UserHeader />
    <DevAside />
    <div style="display: inline">
      <div class="scroll" style="display: inline">
        <DevMain :dishes="dishes" />
      </div>
      <div
        style="
          background-color: aqua;
          width: 20%;
          height: 100vh;
          display: inline;
        "
      ></div>
    </div>
  </div>
</template>

<script>
import DevAside from "./components/DevAside.vue";
import UserHeader from "./components/UserHeader.vue";
import DevMain from "./components/DevMain.vue";

export default {
  name: "App",
  components: {
    UserHeader,
    DevAside,
    DevMain,
  },
  data() {
    return {
      dishes: [
        {
          name: "Waakye",
          id: 1,
          kitchen: "Auntie Muni's Kitchen",
          url: "/images/1.jpg",
        },
        {
          name: "Rice",
          id: 2,
          kitchen: "Aunt Macy's Kitchen",
          url: "/images/2.jpg",
        },
        {
          name: "Jollof",
          id: 3,
          kitchen: "Aunt Macy's Kitchen",
          url: "/images/3.jpg",
        },
        {
          name: "Banku",
          id: 4,
          kitchen: "Aunt Macy's Kitchen",
          url: "/images/4.jpg",
        },
        {
          name: "Fufu",
          id: 5,
          kitchen: "Aunt Macy's Kitchen",
          url: "/images/5.jpg",
        },
        {
          name: "Ampesi",
          id: 6,
          kitchen: "Aunt Macy's Kitchen",
          url: "/images/6.jpg",
        },
        {
          name: "Chicken and Fries",
          id: 7,
          kitchen: "KFC",
          url: "/images/7.jpg",
        },
      ],
    };
  },
};
</script>
