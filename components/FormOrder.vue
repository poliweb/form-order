<template>
  <div>
    <section class="text-gray-600 body-font relative">
  <div class="container px-0 sm:py-16 md:px-5 py-24 mx-auto flex sm:flex-col md:flex-row  flex-wrap max-w-6xl">
    <div class="md:hidden flex flex-row justify-between bg-white w-full pt-10 pb-2.5 px-5">
        <span class="text-lg font-bold">Reduslim</span>
        <span class="text-lg font-bold">ECO</span>
      </div>
    <div class="w-full lg:w-1/2 pl-14 md:px-0 pr-10 bg-white md:bg-gray-300  overflow-hidden relative my-auto">
      <img src="~/assets/img/foto-forms.jpg" alt="" class="w-full hidden md:block">
      <img src="~/assets/img/fotoFormsMobilka.svg" alt="" class="w-full md:hidden">
    </div>
    <div class="lg:w-1/2 md:w-full  bg-white flex flex-col md:ml-auto w-full md:py-0 mt-0 md:mt-0">
      <h2 class="text-gray-900 text-lg mb-1 text-3xl font-extrabold text-center title-font py-7 sm:px-5 md:px-10 bg-title">Сделай шаг к выздоровлению</h2>
      <div class="inputGrups">
        <div class="relative mb-4 text-left">
          <label for="name" class="leading-7 text-xs font-extrabold uppercase  text-gray-600">Ваше <span class="green">имя</span></label>
          <input type="text" id="name" name="name" placeholder="Алексей" class="w-full inputForm focus:border-indigo-500 focus:ring-2 focus:ring-indigo-200 text-sm outline-none text-gray-700 py-4 px-5 leading-5 transition-colors duration-200 ease-in-out">
        </div>
        <div class="relative mb-4 text-left">
          <label for="tel" class="leading-7 text-xs font-extrabold uppercase text-gray-600">Ваш <span class="green">телефон</span></label>
          <div class="flex justify-between">
          <input type="tel" id="phone" name="phone" placeholder="+7 (123) 456 78-90" class="w-full inputForm focus:border-indigo-500 focus:ring-2 focus:ring-indigo-200 text-sm outline-none text-gray-700 py-4 px-5 leading-5 transition-colors duration-200 ease-in-out">
          <SelectForm/>
          </div>
        </div>

            <!-- ========================= -->

            <!-- ========================= -->

        <button class="w-full mt-6 inline-flex items-center justify-center gap-2  text-white bg-green border-0 py-2 px-6 focus:outline-none hover:bg-green-500 rounded text-lg">Заказать <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3" />
</svg></button>
        <div class="flex flex-row justify-center items-center md:hidden h-10 mt-7">
          <div class="text-sm font-bold">Trusted</div>
          <div class="w-3 h-4 mx-5"><img src="~/assets/img/lock.svg" alt=""></div>
          <div class="text-sm font-bold">Secure</div>
        </div>
        <!-- <p class="text-xs text-gray-500 mt-3">Chicharrones blog helvetica normcore iceland tousled brook viral artisan.</p> -->
      </div>
    </div>
  </div>
</section>
  </div>
</template>

<script>
export default {

}
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
@apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/

body {
  font-family: 'Montserrat', sans-serif;
  background: #E5E5E5;;
}

.bg-title {
  background-color: #F8F8F8;
}

.green {
  color: #428A60;
}

.bg-green {
  background-color: #428A60;
}

.inputGrups {
/* padding-top: 52px;
padding-left: 110px;
padding-right: 110px; */
padding: 52px 110px 40px 110px;
}

.inputForm {
  background: #F8F8F8;
  border: 1px solid #E4E4E4;
  box-sizing: border-box;
  border-radius: 5px;

}

@media only screen and (max-width: 640px) {
  /* place here CSS for when the screen is more than 640px wide */
  /* .sm\:margin_b_0 {
    margin-bottom: 0px;
  } */
  .inputGrups {
    padding: 52px 20px 0px 20px;
  }

  .bg-title {
  background-color: #FFF;
}

}

</style>
