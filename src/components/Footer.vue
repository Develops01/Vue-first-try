<script setup></script>

<template>
  <footer
    class="relative w-full m-auto p-12 flex flex-col lg:flex-row rounded-t-3xl bg-[#BD6678]"
  >
    <div class="w-full">
      <div class="p-8 w-full lg:max-w-[30rem]">
        <h2 class="text-2xl text-white font-semibold mb-4">
          اولین نفری باشید که از مقالات جدید مطلع می شوید
        </h2>
        <form>
          <div class="mb-4">
            <label
              for="email"
              class="block text-white text-xl font-medium mb-2"
            >
              آدرس ایمیل
            </label>
            <input
              type="email"
              id="email"
              name="email"
              class="w-full border-2 border-gray-300 p-2 rounded focus:outline-none focus:border-blue-500"
              placeholder="آدرس ایمیل خود را وارد کنید"
              required
            />
          </div>
          <button
            type="submit"
            class="bg-[#D3AE36] cursor-pointer px-5 py-2 text-white hover:text-slate-700 rounded-lg hover:bg-[#ffd13a] hover:shadow-lg transition-all duration-500"
          >
            ارسال
          </button>
        </form>
      </div>
    </div>
    <div class="p-8 w-full">
      <h2 class="text-2xl font-semibold mb-4 text-white">بخش های اصلی</h2>
      <ul class="list-disc pl-6">
        <li class="text-white">نمونه کارها</li>
        <li class="text-white">مقالات</li>
        <li class="text-white">همکاری</li>
        <li class="text-white">راهکارها</li>
      </ul>
    </div>
    <div class="flex w-full p-5 flex-col gap-5">
      <h2 class="text-2xl font-semibold text-white">خدمات مشتریان</h2>
      <div class="flex flex-row gap-4">
        <img
          src="https://landin.ir/landing/brandist/img/i-location.svg"
          alt=""
        />
        <p class="text-white w-full">
          تهــران، اتوبان لشگری، بعد از ایستگاه مترو بیمه پلاک ۳۱، کارخانه
          نوآوری آزادی، ساختمان روز اول
        </p>
      </div>
      <div class="flex flex-row gap-4">
        <img src="https://landin.ir/landing/brandist/img/i-email.svg" alt="" />
        <p class="text-white w-full">info@brandist.com</p>
      </div>
      <div class="flex flex-row gap-4">
        <img src="https://landin.ir/landing/brandist/img/i-phone.svg" alt="" />
        <p class="text-white w-full">۰۲۱-۴۳۰۴۹۰۰۰</p>
      </div>
    </div>
    <div>
      <img
        class="shadow w-36 my-4 bg-[#aa5e6d]"
        src="../assets/arad.png"
        alt="logo"
      />
      <p class="text-white w-full">
        کلیه حقوق این وب سایت متعلق به شرکت بازاریابی و برندینگ برندیست است
      </p>
    </div>
    <div class="absolute bottom-6 left-6 flex flex-row gap-2">
      <a href="#">
        <img
          src="https://landin.ir/landing/brandist/img/i-ins.svg"
          alt="instagram"
      /></a>
      <a href="#">
        <img
          src="https://landin.ir/landing/brandist/img/i-te.svg"
          alt="instagram"
      /></a>
      <a href="#">
        <img
          src="https://landin.ir/landing/brandist/img/i-tw.svg"
          alt="instagram"
      /></a>
      <a href="#">
        <img
          src="https://landin.ir/landing/brandist/img/i-in.svg"
          alt="instagram"
      /></a>
    </div>
  </footer>
</template>

<style scoped></style>
