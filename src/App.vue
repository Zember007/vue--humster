<script setup>
import { ref } from 'vue';

const SelectIcon = ref('')
const Finish = ref('')

</script>

<template>
  <div v-if="!Finish" class="container mx-auto p-20 flex flex-col gap-[60px]">
    <div class="flex flex-col gap-2 text-center">
      <h2 class="font-semibold text-white text-[50px]">Бесплатная накрутка <span v-if="SelectIcon">{{ SelectIcon
          }}</span><span v-else>без заданий</span></h2>
      <span class="text-[#FD346E] text-[20px] font-normal">Доступная каждые 30 минут - Вы можете оформить заказ
        неограниченное количество раз</span>
    </div>
    <div class="flex gap-[30px]" v-if="!SelectIcon">
      <div
        class="grid grid-cols-[auto_auto_auto_auto_auto] gap-[14px] bg-[#2F2F55] rounded-[15px] px-[60px] py-[54px] w-full">
        <button @click="SelectIcon = 'Instagram'"
          class="h-[150px] w-[150px] flex items-center justify-center rounded-[15px] icon-gradient">
          <img src="/icons/Instagram.svg" alt="telegram">
        </button>
        <button @click="SelectIcon = 'Telegram'"
          class="h-[150px] w-[150px] flex items-center justify-center rounded-[15px] icon-gradient">
          <img src="/icons/Telegram.svg" alt="telegram">
        </button>
        <button @click="SelectIcon = 'VK'"
          class="h-[150px] w-[150px] flex items-center justify-center rounded-[15px] icon-gradient">
          <img src="/icons/VK.svg" alt="telegram">
        </button>
        <button @click="SelectIcon = 'Youtube'"
          class="h-[150px] w-[150px] flex items-center justify-center rounded-[15px] icon-gradient">
          <img src="/icons/Youtube.svg" alt="telegram">
        </button>
        <button @click="SelectIcon = 'TikTok'"
          class="h-[150px] w-[150px] flex items-center justify-center rounded-[15px] icon-gradient">
          <img src="/icons/TikTok.svg" alt="telegram">
        </button>
        <button @click="SelectIcon = 'Facebook'"
          class="h-[150px] w-[150px] flex items-center justify-center rounded-[15px] icon-gradient">
          <img src="/icons/Facebook.svg" alt="telegram">
        </button>
        <button @click="SelectIcon = 'Twitch'"
          class="h-[150px] w-[150px] flex items-center justify-center rounded-[15px] icon-gradient">
          <img src="/icons/Twitch.svg" alt="telegram">
        </button>
        <button @click="SelectIcon = 'Twitter'"
          class="h-[150px] w-[150px] flex items-center justify-center rounded-[15px] icon-gradient">
          <img src="/icons/Twitter.svg" alt="telegram">
        </button>
        <button class="row-span-2 col-span-2 h-full w-auto relative">
          <img class="h-full w-auto absolute top-0 scale-[1.3] translate-x-[15%] translate-y-[8%]" src="/3.webp"
            alt="humster">
        </button>
        <button @click="SelectIcon = 'Likee'"
          class="h-[150px] w-[150px] flex items-center justify-center rounded-[15px] icon-gradient">
          <img src="/icons/Likee.svg" alt="telegram">
        </button>
        <button @click="SelectIcon = 'Soundcloud'"
          class="h-[150px] w-[150px] flex items-center justify-center rounded-[15px] icon-gradient">
          <img src="/icons/Soundcloud.svg" alt="telegram">
        </button>
        <button @click="SelectIcon = 'Sharethis'"
          class="h-[150px] w-[150px] flex items-center justify-center rounded-[15px] icon-gradient">
          <img src="/icons/Sharethis.svg" alt="telegram">
        </button>
      </div>
      <div class="relative min-h-full w-[72%] rounded-[15px] overflow-hidden">
        <img class="h-full w-auto" src="/video.webp" alt="video">
        <a href="#"
          class="overflow-hidden top-[50%] left-[50%] translate-y-[-50%] translate-x-[-50%] absolute rounded-[100%]">
          <svg width="83" height="83" viewBox="0 0 83 83" fill="none" xmlns="http://www.w3.org/2000/svg">
            <circle cx="40" cy="40" r="24.5" fill="white" />
            <path
              d="M41.5 0C33.2921 0 25.2685 2.43393 18.4438 6.99401C11.6192 11.5541 6.30005 18.0355 3.15902 25.6186C0.0179811 33.2018 -0.803857 41.546 0.797429 49.5962C2.39872 57.6464 6.35121 65.041 12.1551 70.8449C17.959 76.6488 25.3536 80.6013 33.4038 82.2026C41.454 83.8039 49.7982 82.982 57.3814 79.841C64.9645 76.6999 71.4459 71.3808 76.006 64.5561C80.5661 57.7315 83 49.7079 83 41.5C83 30.4935 78.6277 19.9378 70.8449 12.1551C63.0622 4.37231 52.5065 0 41.5 0ZM56.44 47.5867L37.9956 58.1C36.9342 58.671 35.7435 58.9586 34.5386 58.9351C33.3336 58.9117 32.155 58.5779 31.1167 57.966C30.0784 57.3541 29.2153 56.4848 28.611 55.4421C28.0067 54.3994 27.6814 53.2184 27.6667 52.0133V30.9867C27.6637 29.7549 27.9854 28.5442 28.5994 27.4763C29.2133 26.4085 30.0979 25.5213 31.1638 24.9042C32.2298 24.287 33.4396 23.9617 34.6714 23.961C35.9031 23.9602 37.1133 24.2841 38.18 24.9L56.6245 35.4133C57.6769 36.0515 58.5441 36.9539 59.1399 38.0309C59.7357 39.108 60.0394 40.3221 60.0207 41.5528C60.0021 42.7835 59.6618 43.988 59.0336 45.0464C58.4055 46.1049 57.5113 46.9807 56.44 47.5867Z"
              fill="url(#paint0_linear_1_223)" />
            <defs>

              <linearGradient id="paint0_linear_1_223" x1="41.5" y1="0" x2="41.5" y2="83"
                gradientUnits="userSpaceOnUse">
                <stop stop-color="#8478FF" />
                <stop offset="1" stop-color="#5B4EFF" />
              </linearGradient>
            </defs>
          </svg>
        </a>
      </div>
    </div>
    <div v-if="SelectIcon" class="flex flex-col gap-[30px] bg-[url('/bg.png')] rounded-[15px] px-[90px] py-[54px]">
      <div class="flex gap-20">
        <div class="flex flex-col gap-[20px]">
          <div class="flex items-center gap-[15px]">
            <div class="h-[60px] w-[60px] flex items-center justify-center rounded-[15px] icon-gradient">
              <img :src="'/icons/' + SelectIcon + '.svg'" alt="telegram">
            </div>
            <span class="text-white text-[18px] font-semibold">Выбранная услуга</span>
          </div>
          <div class="flex items-center gap-[15px]">
            <div class="h-[60px] w-[60px] flex items-center justify-center rounded-[15px] icon-gradient">
              <img src="/icons/share.svg" alt="telegram">
            </div>
            <span class="text-white text-[18px] font-semibold">Укажите ссылку</span>
          </div>

        </div>
        <div class="flex flex-col gap-6 grow">
          <input placeholder="Укажите ссылку на пост Telegram. Пример: https://t.me/***/***" type="text"
            class="placeholder:text-white w-full border-solid border border-[#68679C] bg-[#33325c] rounded-[15px] px-[24px] py-[20px] text-white text-[16px]">
          <div class="flex px-6 gap-2 items-center">
            <label class="flex items-center cursor-pointer relative">
              <input type="checkbox" checked
                class="border-solid block peer h-5 w-5 cursor-pointer bg-[#33325c] transition-all appearance-none bg-transparent rounded shadow hover:shadow-md border border-[#68679C]"
                id="check" />
              <span
                class="block absolute text-white opacity-0 peer-checked:opacity-100 top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 pointer-events-none">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-3.5 w-3.5" viewBox="0 0 20 20" fill="currentColor"
                  stroke="currentColor" stroke-width="1">
                  <path fill-rule="evenodd"
                    d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
                    clip-rule="evenodd"></path>
                </svg>
              </span>
            </label>
            <span class="text-[#9c97e3] text-[12px] font-normal">Заказывая бесплатную накрутку Вы соглашаетесь, что
              ознакомились с условиями по бесплатной накрутке.</span>
          </div>
        </div>
      </div>
      <div class="relative w-full rounded-[15px] block-gradient px-[125px] py-[30px] flex justify-end">
        <div class="absolute flex bottom-[-50%] left-[-100px] ">
          <div class="translate-x-[100px]"><img src="/2.webp" alt="humster"></div>
          <div class="relative z-10"><img src="/1.webp" alt="humster"></div>
          <div class="translate-x-[-35%] "><img src="/3.webp" alt="humster"></div>
        </div>
        <div class="flex flex-col gap-[36px] items-center">
          <span class="font-light text-[24px] text-[#b0b7c3]">Следующий заказ можно оформить через</span>
          <div class="gap-[25px] flex items-center text-white text-[64px] font-extralight">
            <span
              class="rounded-[15px] border-solid border-[2px] border-[#5F52FF] w-[110px] h-[85px] flex items-center justify-center">0</span>
            :
            <span
              class="rounded-[15px] border-solid border-[2px] border-[#5F52FF] w-[110px] h-[85px] flex items-center justify-center">0</span>
            :
            <span
              class="rounded-[15px] border-solid border-[2px] border-[#5F52FF] w-[110px] h-[85px] flex items-center justify-center">0</span>
          </div>
          <div class="flex gap-[16px]">
            <button @click="Finish = 'successfull'" class="rounded-[28px] px-[64px] py-[18px] icon-gradient text-white font-normal">Заказать</button>
            <a href="#"
              class="bg-[#33325c] rounded-[28px] border-solid border border-[#68679C] flex items-center gap-[12px] px-[25px] py-[18px]">
              <svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path
                  d="M10 0C8.02219 0 6.08879 0.58649 4.4443 1.6853C2.79981 2.78412 1.51809 4.3459 0.761209 6.17316C0.00433279 8.00042 -0.1937 10.0111 0.192152 11.9509C0.578004 13.8907 1.53041 15.6725 2.92894 17.0711C4.32746 18.4696 6.10929 19.422 8.0491 19.8078C9.98891 20.1937 11.9996 19.9957 13.8268 19.2388C15.6541 18.4819 17.2159 17.2002 18.3147 15.5557C19.4135 13.9112 20 11.9778 20 10C20 7.34783 18.9464 4.80429 17.0711 2.92893C15.1957 1.05357 12.6522 0 10 0ZM13.6 11.4667L9.15556 14C8.89981 14.1376 8.6129 14.2069 8.32254 14.2012C8.03219 14.1956 7.7482 14.1152 7.498 13.9677C7.2478 13.8203 7.03984 13.6108 6.89422 13.3595C6.7486 13.1083 6.67022 12.8237 6.66667 12.5333V7.46666C6.66596 7.16986 6.74348 6.87811 6.89142 6.6208C7.03936 6.36349 7.2525 6.14972 7.50936 6.00101C7.76622 5.8523 8.05774 5.77391 8.35455 5.77373C8.65135 5.77355 8.94296 5.85159 9.2 6L13.6444 8.53333C13.8981 8.68711 14.107 8.90456 14.2506 9.16408C14.3942 9.42361 14.4673 9.71618 14.4628 10.0127C14.4583 10.3093 14.3763 10.5995 14.225 10.8546C14.0736 11.1096 13.8582 11.3206 13.6 11.4667Z"
                  fill="white" />
              </svg>
              <span class="text-white font-normal">Видео-инструкция</span>
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div v-if="Finish"
    class="bg-[url('/bg.png')] rounded-[15px] border-[25px] justify-center border-solid border-[#FD346E] px-[200px] py-[80px] flex gap-[30px]">
    <div class="flex flex-col gap-2 ">
      <h2 class="font-semibold text-white text-[50px]">Ваш заказ успешно отправлен</h2>
      <span class="font-normal text-[20px] text-[#9c97e3]">По истечению 30 минут, вы сможете снова заказать любую
        бесплатную услугу.</span>
    </div>
    <div class="relative w-[350px]">
      <div class="absolute w-[350px] h-[350px] top-[50%] translate-y-[-50%]">
        <img src="/1.webp" alt="humster">
      </div>
    </div>
  </div>

</template>

<style scoped>
.icon-gradient {
  background: linear-gradient(180deg, #8579ff 0%, #5a4dff 100%);
}

.block-gradient {
  background: linear-gradient(90deg, rgba(51, 50, 92, 0) 0%, #33325c 100%);
}
</style>
