<script setup></script>

<template>
  <div
    class="m-auto shadow-lg flex flex-col justify-center gap-5 p-5 my-12 lg:p-12 items-center w-10/12 bg-[#BD6678] rounded"
  >
    <h3 class="text-white text-2xl lg:text-5xl">همین حالا شروع کنید</h3>
    <p class="text-white lg:text-xl">
      طراحی و استقرار سیستم مارکتینگ آتومیشن را به متخصصان برندیست بسپارید
    </p>
    <form class="w-10/12 flex flex-col gap-5 justify-center items-end">
      <input
        class="p-2 w-full rounded-2xl outline-none"
        placeholder="نام و نام خانوادگی"
        type="text"
        required
      />
      <input
        class="p-2 w-full rounded-2xl outline-none"
        placeholder="شماره تماس"
        type="number"
        required
      />
      <input
        class="p-2 w-full rounded-2xl outline-none"
        placeholder="نام شرکت"
        type="text"
        required
      />
      <input
        class="p-2 w-full rounded-2xl outline-none"
        placeholder="ایمیل"
        type="email"
        required
      />
      <input
        class="bg-[#D3AE36] cursor-pointer text-white hover:text-slate-700 rounded-lg p-2 hover:bg-[#ffd13a] hover:shadow-lg transition-all duration-500"
        value="درخواست مشاوره"
        type="submit"
      />
    </form>
  </div>
</template>

<style scoped></style>
