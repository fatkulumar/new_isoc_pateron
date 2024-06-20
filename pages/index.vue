<style>
.bg1-image {
  position: relative; /* Pastikan elemen ini memiliki posisi relatif */
}

.bg1-image::before {
  content: "";
  position: absolute;
  inset: 0;
  background-image: url("/bg2.png");
  background-size: cover;
  background-position: center;
  opacity: 0.1;
  z-index: -1;
}
</style>

<style scoped>
.swiper-container {
  position: relative;
}

.slide-content {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 300px;
  font-size: 24px;
}

.swiper-button-next,
.swiper-button-prev {
  color: #000; /* Warna tombol */
  background: rgba(255, 255, 255, 0.8); /* Warna latar belakang */
  border-radius: 50%; /* Membuat tombol berbentuk bulat */
  width: 40px; /* Ukuran tombol */
  height: 40px; /* Ukuran tombol */
  display: flex;
  align-items: center;
  justify-content: center;
}

.swiper-button-next::after,
.swiper-button-prev::after {
  font-size: 20px; /* Ukuran ikon panah */
}

.swiper-button-next:hover,
.swiper-button-prev:hover {
  background: rgba(255, 255, 255, 1); /* Warna latar belakang saat di-hover */
}
</style>

<script>
  import 'swiper/css';
  import 'swiper/css/navigation';
  import 'swiper/css/pagination';
  import 'swiper/css/scrollbar';
</script>

<template>
  <section class="pt-16 bg1-image">
    <div class="md:grid grid-cols-2 gap-4 mx-auto container ">
    <div class="p-6 rounded" >
      <h1 class="text-4xl font-bold mb-4 text-center">Welcome TO ISOC</h1>
      <p class="italic text-center text-gray-400">
        “inspire, challenge, and empower the scientists of tomorrow”
      </p>
      <p class="text-center mt-10">
        Encouraging the role of science and education in achieving sustainable
        development goals, empowering students to become responsible global
        citizens.
      </p>
      <nuxt-link to="/accounts/login"
        class="w-2/4 justify-center flex mx-auto text-white py-3 rounded-md text-center bg-gray-600"
      >
        Let's Join Now
      </nuxt-link>
    </div>
    <div class="p-6 rounded">
      <img class="mx-auto" src="/body/welcome.png" />
    </div>
  </div>
  </section>

  <section class="py-0">
    <div class="flex flex-row justify-center">
      <div
        class="inline-block uppercase text-center bg-green-300 font-bold mx-auto px-4 py-2 rounded-md border-2 border-black"
      >
        current event
      </div>
    </div>
    <div class="bg-green-700 md:mx-3 rounded-3xl">
      <div class="lg:grid grid-cols-2 p-6">
        <div>
          <img
            class="border-8 border-gray-300"
            src="/body/event.png"
            alt=""
          />
          <p
            class="bg-white rounded-xl py-2 my-1 text-xs md:text-md text-center uppercase font-bold"
          >
            International Science Olympiad Contest 4.0
          </p>
        </div>
        <div>
          <p class="md:text-2xl text-center text-white py-4 font-bold">
            Registration Will Be Ended In :
          </p>
          <div class="flex justify-evenly my-4">
            <div class="bg-gray-400">
              <p class="px-4 pt-3 text-4xl">40</p>
              <p class="uppercase text-center pb-2">days</p>
            </div>

            <div class="bg-gray-400">
              <p class="px-4 pt-3 text-4xl p-2 md:p-0">40</p>
              <p class="uppercase text-center pb-2">hours</p>
            </div>

            <div class="bg-gray-400">
              <p class="px-4 pt-3 text-4xl p-2 md:p-0">40</p>
              <p class="uppercase text-center pb-2">minutes</p>
            </div>

            <div class="bg-gray-400">
              <p class="px-4 pt-3 text-4xl p-2 md:p-0">40</p>
              <p class="uppercase text-center pb-2">seconds</p>
            </div>
          </div>

          <div class="grid grid-cols-2 gap-4 mt-16 mx-4">
            <div
              class="bg-purple-300 flex items-center justify-center text-black border-2 border-black rounded-md py-2 md:px-16"
            >
              Register
            </div>
            <div
              class="bg-purple-300 flex items-center justify-center text-black border-2 border-black rounded-md py-2"
            >
              Guidline
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section class="py-12 lg:mx-3" id="about">
    <div class="lg:grid grid-cols-2 gap-16">
        <div class="bg-gray-400 p-16 gap-16 flex flex-wrap md:flex-mowrap justify-center">

            <div class="bg-green-600 border-8 w-48">
              <img class="flex justify-center mx-auto py-1" src="/body/earth.png" alt="">
              <p class="font-bold text-white text-center px-2">
                Worldwide Recognition and Prestige
              </p>
            </div>
            <div class="bg-green-600 border-8 w-48">
              <img class="flex justify-center mx-auto py-1" src="/body/school.png" alt="">
              <p class="font-bold text-white text-center px-2">
                Worldwide Recognition and Prestige
              </p>
            </div>

            <div class="bg-green-600 border-8 w-48">
              <img class="flex justify-center mx-auto py-1" src="/body/people.png" alt="">
              <p class="font-bold text-white text-center px-2">
                Worldwide Recognition and Prestige
              </p>
            </div>
            <div class="bg-green-600 border-8 w-48">
              <img class="flex justify-center mx-auto py-1" src="/body/female_student.png" alt="">
              <p class="text font-bold text-white text-center px-2">
                Worldwide Recognition and Prestige
              </p>
            </div>

            

            <!-- <div class="bg-green-600 border-8">
              <img class="flex justify-center mx-auto py-1" src="/body/people.png" alt="">
              <p class="font-bold text-white text-center px-2">
                Worldwide Recognition and Prestige
              </p>
            </div>
            <div class="bg-green-600 border-8">
              <img class="flex justify-center mx-auto py-1" src="/body/female_student.png" alt="">
              <p class="font-bold text-white text-center px-2">
                Worldwide Recognition and Prestige
              </p>
            </div> -->

            <!-- <div class="flex gap-12 pt-6">
              <div class="bg-green-600 border-8">
                <img class="flex justify-center mx-auto" src="/body/earth.png" alt="">
                <p class="font-bold text-white text-center px-2">
                  Worldwide Recognition and Prestige
                </p>
              </div>
              <div class="bg-green-600 border-8">
                <img class="flex justify-center mx-auto" src="/body/earth.png" alt="">
                <p class="font-bold text-white text-center px-2">
                  Worldwide Recognition and Prestige
                </p>
              </div>
            </div> -->
        </div>
      <div class="mx-2 pt-12 lg:pt-0 bg1-image">
        <p class="text-4xl uppercase font-bold">why isoc olympiad</p>
        <p class="text-justify mb-2">
          BE PART OF ISOC OLYMPIAD ISOC is a leading science institution that has been at the forefront of innovation since its inception. ISOC is dedicated to empowering students since young age in order to support themselves on facing future challenges with confidence. We specialize in identifying each child's unique abilities and potential, preparing them to excel in experiencing today's competitive landscape. Through the olympiad events, our main goals are : 1. to provide great help on educational terms 2. to inspire students for exploring scientific concepts in depth 3. encouraging the development of their reasoning analytical and problem-solving abilities. Join us on the journey to find your passion and growth with ISOC.
        </p>
      </div>
    </div>
  </section>

  <section id="benefit" class="bg1-image">
    <div class="flex flex-row justify-center">
      <div
        class="inline-block uppercase text-center font-bold mx-auto rounded-md border-2 border-black lg:text-4xl px-16 py-2"
      >
        benefits
      </div>
    </div>
    <div class="flex flex-col lg:flex-row justify-center mx-auto lg:justify-evenly gap-12 py-12 bg1-image">
      <div class="lg:w-2/12 flex flex-col items-center">
        <img src="/body/trophy.png" alt="Trophy">
        <p class="text-center text-2xl text-blue-800 uppercase mt-2">Trophy</p>
      </div>
      <div class="lg:w-2/12 flex flex-col items-center">
        <img src="/body/money.png" alt="Money">
        <p class="text-center text-2xl text-red-500 uppercase mt-2">Money</p>
      </div>
      <div class="lg:w-2/12 flex flex-col items-center">
        <img src="/body/medal.png" alt="Medal">
        <p class="text-center text-2xl text-yellow-500 uppercase mt-2">Medal</p>
      </div>
    </div>
    
    <div class="flex flex-col lg:flex-row justify-center mx-auto lg:justify-evenly gap-0 py-0">
      <div class="lg:w-2/12 flex flex-col items-center">
        <img src="/body/certificate.png" alt="">
        <p class="text-center text-2xl text-yellow-400 uppercase mt-2">certificate</p>
      </div>
      <div class="lg:w-2/12 flex flex-col items-center">
        <img src="/body/merchandise.png" alt="">
        <p class="text-center text-2xl text-blue-800 uppercase mt-2">merchandise</p>
      </div>
    </div>
  </section>

  <section class="pt-24 bg1-image">
    <div class="flex flex-row justify-center">
      <div
        class="inline-block uppercase text-center bg-white font-bold mx-auto rounded-md border-2 border-black lg:text-4xl px-16 py-2 text-wrap"
      >
        isoc participant records
      </div>
    </div>
    <div class="flex flex-col lg:flex-row justify-center mx-auto lg:justify-evenly gap-12 py-12">
      <div class="lg:w-2/12 flex flex-col items-center">
        <img src="/body/planet.png" alt="">
        <p class="text-center text-2xl text-blue-800 uppercase mt-2">planet</p>
      </div>
      <div class="lg:w-2/12 flex flex-col items-center">
        <img src="/body/school.png" alt="">
        <p class="text-center text-2xl text-red-500 uppercase mt-2">school</p>
      </div>
      <div class="lg:w-2/12 flex flex-col items-center">
        <img src="/body/student.png" alt="">
        <p class="text-center text-2xl text-yellow-500 uppercase mt-2">student</p>
      </div>
    </div>
  </section>
  
  <section class="lg:pt-24">
    <div class="flex flex-row justify-center">
      <div
        class="inline-block uppercase text-center bg-white font-bold mx-auto rounded-md border-2 border-black lg:text-4xl px-16 py-2"
      >
        isoc 5.0 timeline
      </div>
    </div>
    <div class="flex-col lg:flex-row mx-auto lg:justify-evenly gap-2 lg:gap-12 py-12 flex justify-center items-center">
      <div class="lg:w-3/12 bg-gradient-to-t from-blue-600 to-red-400 rounded-xl lg:py-2 shadow-md flex justify-center items-center">
        <div class="px-24 lg:px-0">
          <p class="text-center lg:text-3xl uppercase mt-2 text-white font-bold">registration close</p>
          <p class="text-center lg:text-3xl uppercase mb-2 text-white font-bold">july, 24 2024</p>
        </div>
      </div>
      <div class="lg:w-3/12 bg-white rounded-xl bg-gradient-to-t from-white to-gray-300 shadow-md flex justify-center items-center">
      <div class="px-32 lg:px-0">
          <p class="text-center lg:text-3xl uppercase mt-2 text-black font-bold">final round</p>
          <p class="text-center lg:text-3xl uppercase mb-2 text-black font-bold">july, 26 2024</p>
        </div>
      </div>
      <div class="lg:hidden lg:w-3/12 bg-blue-600 rounded-xl py-2 bg-gradient-to-r from-yellow-300 to-red-300 shadow-md  flex justify-center items-center">
        <div class="px-24 lg:px-0">
          <p class="text-center lg:text-3xl uppercase mt-2 text-black font-bold">open registration</p>
          <p class="text-center lg:text-3xl uppercase mb-2 text-black font-bold">july, 24 2024</p>
        </div>
      </div>
      <div class="lg:hidden lg:w-3/12 bg-blue-600 rounded-xl bg-gradient-to-r from-red-400 to-blue-900 sm:flex justify-center items-center py-2">
        <div class="px-24 lg:px-0">
          <p class="text-center lg:text-3xl uppercase mt-2 text-white font-bold">preliminary round</p>
          <p class="text-center lg:text-3xl uppercase mb-2 text-white font-bold">july, 26 2024</p>
        </div>
      </div>
      <div class="lg:hidden lg:w-3/12 bg-blue-600 rounded-xl bg-gradient-to-r from-gray-400 to-gray-200 sm:flex justify-center items-center py-4 shadow-md">
        <div class="px-24 lg:px-0">
          <p class="text-center lg:text-3xl uppercase mt-2 text-white font-bold px-4">Announcement</p>
          <p class="text-center lg:text-3xl uppercase mb-2 text-white font-bold">July, 26 2024</p>
        </div>
      </div>
    </div>
    <div class="flex-col lg:flex-row mx-auto lg:justify-evenly gap-2 lg:gap-12 lg:py-12 lg:flex justify-center items-center hidden">
      <div class="lg:w-3/12 bg-blue-600 rounded-xl py-2 bg-gradient-to-r from-yellow-300 to-red-300 shadow-md  flex justify-center items-center">
        <div class="px-24 lg:px-0">
          <p class="text-center lg:text-3xl uppercase mt-2 text-black font-bold">open registration</p> 
          <p class="text-center lg:text-3xl uppercase mb-2 text-black font-bold">july, 24 2024</p>
        </div>
      </div>
      <div class="lg:w-3/12 bg-blue-600 rounded-xl bg-gradient-to-r from-red-400 to-blue-900 flex justify-center items-center py-2">
        <div class="px-24 lg:px-0">
          <p class="text-center lg:text-3xl uppercase mt-2 text-white font-bold">preliminary round</p>
          <p class="text-center lg:text-3xl uppercase mb-2 text-white font-bold">july, 26 2024</p>
        </div>
      </div>
      <div class="lg:w-3/12 bg-blue-600 rounded-xl bg-gradient-to-r from-gray-400 to-gray-200 flex justify-center items-center py-4 shadow-md">
        <div class="px-24 lg:px-0">
          <p class="text-center lg:text-3xl uppercase mt-2 text-white font-bold">Announcement</p>
          <p class="text-center lg:text-3xl uppercase mb-2 text-white font-bold">July, 26 2024</p>
        </div>
      </div>
    </div>
  </section>

  <section class="pt-0" id="category">
    <div class="flex flex-row justify-center">
      <div
        class="inline-block uppercase text-center font-bold mx-auto rounded-md border-2 border-black lg:text-4xl px-16 py-2"
      >
        Category
      </div>
    </div>
    <div class="flex flex-col lg:flex-row justify-center mx-auto lg:justify-evenly gap-12 py-12 bg1-image">
      <div class="lg:w-2/12 flex flex-col items-center">
        <img src="/body/math.png" alt="">
        <p class="text-center text-2xl text-black uppercase">Math</p>
      </div>
      <div class="lg:w-2/12 flex flex-col items-center">
        <img src="/body/science.jpg" alt="">
        <p class="text-center text-2xl text-black uppercase">Science</p>
      </div>
      <div class="lg:w-2/12 flex flex-col items-center">
        <img src="/body/english.png" alt="">
        <p class="text-center text-2xl text-black uppercase">student</p>
      </div>
    </div>
  </section>

  <section class="pt-0">
    <div class="flex flex-row justify-center">
      <div
        class="inline-block uppercase text-center bg-purple-300 font-bold mx-auto rounded-md border-2 border-black lg:text-xl px-16 py-2"
      >
        Let's Register for ISOC 5.0 Now
      </div>
    </div>
    
    <Swiper
     :modules="modules"
      :slides-per-view="1"
      :loop="true"
      :effect="'creative'"
      :autoplay="{
        delay: 8000,
        disableOnInteraction: true,
      }"
      :creative-effect="{
        prev: {
          shadow: false,
          translate: ['-20%', 0, -1],
        },
        next: {
          translate: ['100%', 0, 0],
        },
      }"
    >
  
      <div class="swiper-button-next"></div>
      <div class="swiper-button-prev"></div>

      <SwiperSlide v-for="slide in 10" :key="slide">
        <div class="flex flex-col lg:flex-row justify-center items-center bg1-image slide-content pt-6 md:pt-12">
          <!-- Container untuk konten -->
          <div class="flex flex-col lg:flex-row justify-center items-center py-12 shadow-md rounded-lg max-w-4xl mx-auto p-">
            
            <!-- Gambar -->
            <div class="w-3/12 lg:w-2/12 flex-shrink-0">
              <img src="/body/people_australia.png" alt="Person from Australia" class="w-full h-auto object-cover">
            </div>
            
            <!-- Teks -->
            <div class="flex flex-col items-center text-center max-w-lg lg:max-w-none">
              <p class="w-full lg:w-3/4 xl:w-2/3 lg:text-2xl lg:leading-normal p-4 rounded-md mx-auto">
                “Following ISOC made me more active in studying, and I can be happy to get the opportunity to be a part of this amazing competition. Thank you ISOC”
              </p>
              <p class="mt-4">
                <p>
                  {{ slide }}
                </p>
                ~Emily Abigail Carter~ from Australia
              </p>
            </div>
            
          </div>
        </div>
        
      </SwiperSlide>
    </Swiper>
  </section>


</template>