<script setup lang="ts">
import { onMounted } from 'vue';

//scrollreveal animations
onMounted(() => {
  useScrollReveal('.contact', '40px', 'bottom', 100, 500,)
  useScrollReveal('.contact2', '40px', 'bottom', 200, 500,)
})

</script>

<template>
  <TheTitle heading="Get In Touch" underline-class="justify-start" class="contact" id="contactMe" />
  <div class="text-center contact2 ">
    <div class="w-11/12 sm:w-8/12 md:w-8/12 lg:w-5/12 mx-auto text-center ">
      <div>
        <div class="font-gsans ">
          Are you having a project that you would want me to help you with or you want to hire me, Always feel free to
          reach me
          out through my email, I will respond to you immediately. Thankyou
        </div>
        <div class="flex justify-center my-8 mb-56">
          <NuxtLink to="mailto:jjembatony@gmail.com">
            <div class=" cursor-pointer  textLcolor  bg-opacity-0 border rounded border-mycyan">
              <div class="text-center pt-3 pb-3 pr-5 pl-5 font-gsans font-bold">
                Contact me
              </div>
            </div>
          </NuxtLink>

        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.dark-mode .textLcolor {
  color: #00FFE1;
  transition: color .3s ease-in-out;
}

.textLcolor {
  color: #00FFE1;
}

.light-mode .textLcolor {
  transition: color .3s ease-in-out;

  color: rgba(0, 0, 0, 0.8);
}

.light-mode .textLcolor:hover {
  transition: color .3s ease-in-out;
  background-color: #00ffe11a;
  color: #00FFE1;
}

.dark-mode .textLcolor:hover {
  background-color: #00ffe11a;
  transition: background-color .3s ease-in-out;
}
</style>
