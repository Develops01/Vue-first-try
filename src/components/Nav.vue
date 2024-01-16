<script setup>
import { ref, onMounted, onUnmounted } from "vue";
const menuRef = ref(null);
const burgerRef = ref(null);
const bool = ref(true);

const toggleMenu = () => {
  if (bool.value) {
    burgerRef.value.classList.add("open");
    menuRef.value.style.right = 0;
    bool.value = false;
  } else {
    burgerRef.value.classList.remove("open");
    menuRef.value.style.right = "-100%";
    bool.value = true;
  }
};

// Use refs to access DOM elements
onMounted(() => {
  burgerRef.value = document.querySelector(".menu-burger");
  menuRef.value = document.querySelector(".menu");
});

// Attach event listener when the component is mounted
onMounted(() => {
  burgerRef.value.addEventListener("click", toggleMenu);
});

// Cleanup event listener when the component is unmounted
onUnmounted(() => {
  burgerRef.value.removeEventListener("click", toggleMenu);
});
</script>

<template>
  <nav
    class="relative flex flex-row justify-around w-full bg-[#BD6678] p-4 px-10 sm:pb-24"
  >
    <header class="w-full h-14 sticky top-0 z-40 flex-none bg-[#BD6678]">
      <div class="w-full h-full flex items-center px-4">
        <div class="w-1/2 md:w-1/12 h-full flex justify-start items-center">
          <div class="flex md:hidden menu-burger">
            <div class="burger-inner"></div>
          </div>
        </div>
        <div
          class="w-7/12 pt-10 h-full hidden md:flex justify-start items-center"
        >
          <a
            href="#"
            class="text-xl font-semibold hover:text-[#D3AE36] transition-all duration-500 text-white"
            >صفحه اصلی</a
          >
          <a
            href="#"
            class="text-xl font-semibold hover:text-[#D3AE36] transition-all duration-500 text-white mr-8"
            >راهکارها</a
          >
          <a
            href="#"
            class="text-xl font-semibold hover:text-[#D3AE36] transition-all duration-500 text-white mr-8"
            >سرویس ها</a
          >
          <a
            href="#"
            class="text-xl font-semibold hover:text-[#D3AE36] transition-all duration-500 text-white mr-8"
            >همکاری</a
          >
        </div>
      </div>
    </header>

    <div class="menu md:hidden bg-[#BD6678] pt-14">
      <a
        href="#"
        class="w-full h-12 flex items-center text-xl font-semibold text-white px-2"
        >صفحه اصلی</a
      >
      <a
        href="#"
        class="w-full h-12 flex items-center text-xl font-semibold text-white px-2"
        >راهکارها</a
      >
      <a
        href="#"
        class="w-full h-12 flex items-center text-xl font-semibold text-white px-2"
        >سرویس ها</a
      >
      <a
        href="#"
        class="w-full h-12 flex items-center text-xl font-semibold text-white px-2"
        >همکاری</a
      >
    </div>
    <a href="#" class="absolute z-40 top-5 left-8 w-14 md:w-24"
      ><img class="shadow bg-[#aa5e6d]" src="../assets/arad.png" alt="logo"
    /></a>
  </nav>
</template>

<style scoped>
.menu-burger {
  width: 40px;
  height: 40px;
  position: absolute;
  right: -10px;
  justify-content: start;
  align-items: center;
  cursor: pointer;
}

.menu-burger .burger-inner {
  width: 24px;
  height: 3px;
  border-radius: 10px;
  background-color: white;
  transition: all 0.4s ease-in-out;
}

.menu-burger .burger-inner::before,
.menu-burger .burger-inner::after {
  position: absolute;
  content: "";
  width: 24px;
  height: 3px;
  border-radius: 10px;
  background-color: white;
  transition: all 0.4s ease-in-out;
}

.menu-burger .burger-inner::before {
  transform: translateY(-8px);
}
.menu-burger .burger-inner::after {
  transform: translateY(8px);
}

.menu-burger.open .burger-inner {
  transform: translateX(-30px);
  background-color: transparent;
}

.menu-burger.open .burger-inner::before {
  transform: translate(30px, 0) rotate(45deg);
}
.menu-burger.open .burger-inner::after {
  transform: translate(30px, 0) rotate(-45deg);
}
.menu {
  position: fixed;
  width: 200px;
  height: 100%;
  right: -100%;
  transition: all 0.3s ease-in-out;
  z-index: 30;
}
</style>
