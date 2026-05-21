<template>
  <div class="text-white">
    <div class="relative w-full h-screen">
      <div
        class="relative z-10 flex flex-col justify-center px-8 md:px-14 lg:px-22 h-full"
      >
        <motion.div
          :initial="{ opacity: 0, x: -200 }"
          :animate="{ opacity: 1, x: 0 }"
          :transition="{
            type: 'spring',
            stiffness: 100,
            damping: 12,
            delay: 1.2,
          }"
        >
          <span
            class="text-white/80 text-sm md:text-lg md:ml-10 tracking-widest p-1 px-2 border border-amber-400 rounded-full"
          >
            ⚪你好呀! 这里是——
          </span>
          <div
            class="flex flex-wrap items-center text-xl md:text-2xl mt-5 md:mt-6"
          >
            <img
              class="rounded-full size-16 mx-2 md:mx-4 md:size-30"
              src="https://q1.qlogo.cn/g?b=qq&nk=1263115878&s=640"
            />
            <h1
              ref="typeitElement"
              class="font-['ChildFunSans'] font-bold text-shadow-lg text-3xl sm:text-5xl md:text-7xl bg-linear-to-r from-orange-400 via-rose-500 to-pink-600 bg-clip-text text-transparent drop-shadow-lg"
            ></h1>
          </div>
        </motion.div>

        <div class="mt-10 md:mt-15">
          <div
            class="grid grid-cols-2 sm:grid-cols-3 w-full sm:w-4/5 md:w-3/5 lg:w-2/5"
          >
            <motion.img
              src="/home1.webp"
              :initial="{ opacity: 0, x: -100 }"
              :animate="{ opacity: 1, x: 0 }"
              :transition="{ duration: 0.6 }"
              class="w-full self-end hover:scale-125 active:scale-125 transition-all duration-300 ease-in-out"
            />
            <motion.img
              src="/home2.webp"
              :initial="{ opacity: 0, y: -100 }"
              :animate="{ opacity: 1, y: 0 }"
              :transition="{ duration: 0.6 }"
              class="w-full hover:scale-125 active:scale-125 transition-all duration-300 ease-in-out"
            />
            <motion.img
              src="/home4.webp"
              :initial="{ opacity: 0, x: 100 }"
              :animate="{ opacity: 1, x: 0 }"
              :transition="{ duration: 0.6 }"
              class="w-full self-end hover:scale-125 active:scale-125 transition-all duration-300 ease-in-out"
            />
          </div>
          <div class="grid grid-cols-2 w-4/5 sm:w-3/5 md:w-1/2 lg:w-1/3">
            <motion.img
              src="/home3.webp"
              :initial="{ opacity: 0, x: -100 }"
              :animate="{ opacity: 1, x: 0 }"
              :transition="{ duration: 0.6, delay: 0.2 }"
              class="w-full hover:scale-125 active:scale-125 transition-all duration-300 ease-in-out"
            />
            <motion.img
              src="/home5.webp"
              :initial="{ opacity: 0, x: 100 }"
              :animate="{ opacity: 1, x: 0 }"
              :transition="{ duration: 0.6, delay: 0.2 }"
              class="w-full hover:scale-125 active:scale-125 transition-all duration-300 ease-in-out"
            />
          </div>
        </div>
      </div>
    </div>

    <div class="h-screen w-full flex justify-start mt-40">
      <div
        class="flex flex-col items-center justify-center mx-32 max-md:mx-auto"
      >
        <motion.div
          :initial="{ opacity: 0, x: -50 }"
          :whileInView="{ opacity: 1, x: 0 }"
          :transition="{ duration: 0.5, delay: 0 }"
        >
          <h2
            class="font-bold font-['NanoMyongWenFangSong'] font-stretch-extra-expanded tracking-widest text-3xl md:text-4xl bg-linear-to-r from-gray-300 via-gray-400 to-gray-500 bg-clip-text text-transparent"
          >
            About me?
          </h2>
        </motion.div>

        <div class="text-left mt-6 max-w-md space-y-6 mx-8">
          <motion.div
            :initial="{ opacity: 0, x: -50 }"
            :whileInView="{ opacity: 1, x: 0 }"
            :transition="{ duration: 0.5, delay: 0.1 }"
          >
            <p class="text-gray-200 text-sm leading-relaxed">
              这里晨辞！{{ Age }} 岁，在读学生。平时
              <span class="line-through"> 技术佬</span>
              ，鼓捣手机、攒钱旅行、练着摄影。是FURRY，一只蓝白色的狼龙，很
              <span class="line-through"> 可爱</span> 傻。
            </p>
          </motion.div>

          <div class="space-y-3">
            <motion.div
              :initial="{ opacity: 0, x: -50 }"
              :whileInView="{ opacity: 1, x: 0 }"
              :transition="{ duration: 0.5, delay: 0 }"
            >
              <div class="space-y-1">
                <div class="flex justify-between text-xs text-gray-300">
                  <span class="inline-flex items-center gap-1">
                    <Icon><Html5 /></Icon>HTML5
                  </span>
                  <span class="text-gray-400">35%</span>
                </div>
                <progress
                  class="progress progress-primary w-full h-1.5"
                  value="35"
                  max="100"
                />
              </div>
            </motion.div>
            <motion.div
              :initial="{ opacity: 0, x: -50 }"
              :whileInView="{ opacity: 1, x: 0 }"
              :transition="{ duration: 0.5, delay: 0.05 }"
            >
              <div class="space-y-1">
                <div class="flex justify-between text-xs text-gray-300">
                  <span class="inline-flex items-center gap-1">
                    <Icon><Vuejs /></Icon>Vue
                  </span>
                  <span class="text-gray-400">35%</span>
                </div>
                <progress
                  class="progress progress-primary w-full h-1.5"
                  value="35"
                  max="100"
                />
              </div>
            </motion.div>
            <motion.div
              :initial="{ opacity: 0, x: -50 }"
              :whileInView="{ opacity: 1, x: 0 }"
              :transition="{ duration: 0.5, delay: 0.1 }"
            >
              <div class="space-y-1">
                <div class="flex justify-between text-xs text-gray-300">
                  <span class="inline-flex items-center gap-1">
                    <Icon><Google /></Icon>Go
                  </span>
                  <span class="text-gray-400">35%</span>
                </div>
                <progress
                  class="progress progress-primary w-full h-1.5"
                  value="35"
                  max="100"
                />
              </div>
            </motion.div>
          </div>
          <div class="space-y-3 mt-10">
            <motion.div
              :initial="{ opacity: 0, x: -50 }"
              :whileInView="{ opacity: 1, x: 0 }"
              :transition="{ duration: 0.5, delay: 0.15 }"
            >
              <div class="space-y-1">
                <div class="flex justify-between text-xs text-gray-300">
                  <span
                    class="inline-flex items-center gap-1 tooltip max-sm:tooltip-right sm:tooltip-bottom"
                    data-tip="玩不好自己手机很难受的"
                    ><Icon><Android /></Icon>玩机</span
                  >
                  <span class="text-gray-400">65%</span>
                </div>
                <progress
                  class="progress progress-secondary w-full h-1.5"
                  value="65"
                  max="100"
                />
              </div>
            </motion.div>
            <motion.div
              :initial="{ opacity: 0, x: -50 }"
              :whileInView="{ opacity: 1, x: 0 }"
              :transition="{ duration: 0.5, delay: 0.2 }"
            >
              <div class="space-y-1">
                <div class="flex justify-between text-xs text-gray-300">
                  <span
                    class="inline-flex items-center gap-1 tooltip max-sm:tooltip-right sm:tooltip-bottom"
                    data-tip="自从摔了一次后就不怎么想骑了"
                    ><Icon><Biking /></Icon>骑行</span
                  >
                  <span class="text-gray-400">25%</span>
                </div>
                <progress
                  class="progress progress-secondary w-full h-1.5"
                  value="25"
                  max="100"
                />
              </div>
            </motion.div>
            <motion.div
              :initial="{ opacity: 0, x: -50 }"
              :whileInView="{ opacity: 1, x: 0 }"
              :transition="{ duration: 0.5, delay: 0.25 }"
            >
              <div class="space-y-1">
                <div class="flex justify-between text-xs text-gray-300">
                  <span
                    class="inline-flex items-center gap-1 tooltip max-sm:tooltip-right sm:tooltip-bottom"
                    data-tip="我渴望外面的世界..."
                    ><Icon><PlaneDeparture /></Icon>旅行</span
                  >
                  <span class="text-gray-400">85%</span>
                </div>
                <progress
                  class="progress progress-secondary w-full h-1.5"
                  value="85"
                  max="100"
                />
              </div>
            </motion.div>
            <motion.div
              :initial="{ opacity: 0, x: -50 }"
              :whileInView="{ opacity: 1, x: 0 }"
              :transition="{ duration: 0.5, delay: 0.3 }"
            >
              <div class="space-y-1">
                <div class="flex justify-between text-xs text-gray-300">
                  <span
                    class="inline-flex items-center gap-1 tooltip max-sm:tooltip-right sm:tooltip-bottom"
                    data-tip="熟练度一般，还得练"
                    ><Icon><Camera /></Icon>摄影</span
                  >
                  <span class="text-gray-400">70%</span>
                </div>
                <progress
                  class="progress progress-secondary w-full h-1.5"
                  value="70"
                  max="100"
                />
              </div>
            </motion.div>
            <motion.div
              :initial="{ opacity: 0, x: -50 }"
              :whileInView="{ opacity: 1, x: 0 }"
              :transition="{ duration: 0.5, delay: 0.35 }"
            >
              <div class="space-y-1">
                <div class="flex justify-between text-xs text-gray-300">
                  <span
                    class="inline-flex items-center gap-1 tooltip max-sm:tooltip-right sm:tooltip-bottom"
                    data-tip="开服人开服魂，方块人一辈子"
                    ><Icon><Xbox /></Icon>Minecraft</span
                  >
                  <span class="text-gray-400">95%</span>
                </div>
                <progress
                  class="progress progress-secondary w-full h-1.5"
                  value="95"
                  max="100"
                />
              </div>
            </motion.div>
            <motion.div
              :initial="{ opacity: 0, x: -50 }"
              :whileInView="{ opacity: 1, x: 0 }"
              :transition="{ duration: 0.5, delay: 0.4 }"
            >
              <div class="space-y-1">
                <div class="flex justify-between text-xs text-gray-300">
                  <span
                    class="inline-flex items-center gap-1 tooltip max-sm:tooltip-right sm:tooltip-bottom"
                    data-tip="可爱的毛绒绒谁不喜欢"
                    ><Icon><AnimalDog16Filled /></Icon>Furry</span
                  >
                  <span class="text-gray-400">95%</span>
                </div>
                <progress
                  class="progress progress-secondary w-full h-1.5"
                  value="95"
                  max="100"
                />
              </div>
            </motion.div>
          </div>
        </div>
      </div>
    </div>

    <div class="h-screen w-full flex justify-start">
      <div
        class="flex flex-col items-center justify-center mx-8 max-md:mx-auto"
      >
        <div class="mockup-code w-full max-w-lg bg-gray-900/75 mb-20">
          <pre data-prefix="$"><code>weather</code></pre>
          <pre
            v-if="weather"
            data-prefix=">"
          ><code>{{ weather.province }} {{ weather.city }}{{ weather.district ? ' · ' + weather.district : '' }}</code></pre>
          <pre
            v-if="weather"
            data-prefix=">"
          ><code>{{ weatherEmoji }} {{ weather.weather }}  {{ weather.temperature }}°C  (体感 {{ weather.feels_like }}°C)</code></pre>
          <pre
            v-if="weather"
            data-prefix=">"
          ><code>{{ weather.wind_direction }} {{ weather.wind_power }}  |  湿度 {{ weather.humidity }}%  |  {{ weather.visibility }}km</code></pre>
          <pre
            v-if="weather && weather.aqi !== undefined"
            data-prefix=">"
          ><code>AQI {{ weather.aqi }} {{ weather.aqi_level }}  |  紫外线 {{ weather.uv_index }}</code></pre>
          <pre
            v-if="weather"
            data-prefix=">"
          ><code>{{ weather.report_time }}</code></pre>
          <pre
            v-else-if="!weatherError"
            data-prefix=">"
            class="text-warning"
          ><code>loading...</code></pre>
          <pre
            v-if="weatherError"
            data-prefix=">"
            class="text-error"
          ><code>获取失败</code></pre>
        </div>
        <motion.div
          :initial="{ opacity: 0, x: -50 }"
          :whileInView="{ opacity: 1, x: 0 }"
          :transition="{ duration: 0.5, delay: 0 }"
        >
          <h2
            class="font-black font-stretch-extra-expanded tracking-widest font-['NanoMyongWenFangSong'] text-3xl md:text-4xl bg-linear-to-r from-gray-300 via-gray-400 to-gray-500 bg-clip-text text-transparent"
          >
            联系/视奸我
          </h2>
        </motion.div>
        <motion.div
          :initial="{ opacity: 0, scaleX: 0 }"
          :whileInView="{ opacity: 1, scaleX: 1 }"
          :transition="{ duration: 0.5, delay: 0.2 }"
          class="flex items-center gap-3 mt-2"
        >
          <div
            class="w-8 h-px bg-linear-to-r from-transparent to-gray-500"
          ></div>
          <span class="text-sm text-gray-400 tracking-widest">CONTACT ME</span>
          <div
            class="w-8 h-px bg-linear-to-l from-transparent to-gray-500"
          ></div>
        </motion.div>
        <div class="grid grid-cols-2 md:grid-cols-4 gap-10 mt-10">
          <motion.div
            :initial="{ opacity: 0, y: 40 }"
            :whileInView="{ opacity: 1, y: 0 }"
            :transition="{ duration: 0.5, delay: 0.3 }"
          >
            <a
              class="btn btn-lg w-36 px-0 font-light text-xl border-transparent bg-[linear-gradient(to_top,transparent_50%,#3b82f6_50%)] bg-size-[100%_200%] bg-bottom hover:bg-top hover:transform-[perspective(800px)_rotateX(5deg)_rotateY(-6deg)_translateY(-3px)] hover:[box-shadow:-6px_10px_25px_rgba(0,0,0,0.35)] active:transform-[perspective(800px)_rotateX(2deg)_rotateY(-2deg)_translateY(-1px)] transition-all duration-350 ease-out"
              href="https://qm.qq.com/q/o2Bzoxg0lq"
              target="_blank"
            >
              <Icon><Qq /></Icon>QQ
            </a>
          </motion.div>
          <motion.div
            :initial="{ opacity: 0, y: 40 }"
            :whileInView="{ opacity: 1, y: 0 }"
            :transition="{ duration: 0.5, delay: 0.4 }"
          >
            <a
              class="btn btn-lg w-36 px-0 font-light text-xl border-transparent bg-[linear-gradient(to_top,transparent_50%,#eab308_50%)] bg-size-[100%_200%] bg-bottom hover:bg-top hover:transform-[perspective(800px)_rotateX(5deg)_rotateY(-6deg)_translateY(-3px)] hover:[box-shadow:-6px_10px_25px_rgba(0,0,0,0.35)] active:transform-[perspective(800px)_rotateX(2deg)_rotateY(-2deg)_translateY(-1px)] transition-all duration-350 ease-out"
              @click="copyEmail"
              onclick="alert('邮箱已复制到剪切板')"
            >
              <Icon><MailBulk /></Icon>EMail
            </a>
          </motion.div>
          <motion.div
            :initial="{ opacity: 0, y: 40 }"
            :whileInView="{ opacity: 1, y: 0 }"
            :transition="{ duration: 0.5, delay: 0.5 }"
          >
            <a
              class="btn btn-lg w-36 px-0 font-light text-xl border-transparent bg-[linear-gradient(to_top,transparent_50%,#db2777_50%)] bg-size-[100%_200%] bg-bottom hover:bg-top hover:transform-[perspective(800px)_rotateX(5deg)_rotateY(-6deg)_translateY(-3px)] hover:[box-shadow:-6px_10px_25px_rgba(0,0,0,0.35)] active:transform-[perspective(800px)_rotateX(2deg)_rotateY(-2deg)_translateY(-1px)] transition-all duration-350 ease-out"
              href="https://b23.tv/KjyGoIk"
              target="_blank"
            >
              <Icon><LiveTvOutlined /></Icon>bilibili
            </a>
          </motion.div>
          <motion.div
            :initial="{ opacity: 0, y: 40 }"
            :whileInView="{ opacity: 1, y: 0 }"
            :transition="{ duration: 0.5, delay: 0.6 }"
          >
            <a
              class="btn btn-lg w-36 px-0 font-light text-xl border-transparent bg-[linear-gradient(to_top,transparent_50%,#7c3aed_50%)] bg-size-[100%_200%] bg-bottom hover:bg-top hover:transform-[perspective(800px)_rotateX(5deg)_rotateY(-6deg)_translateY(-3px)] hover:[box-shadow:-6px_10px_25px_rgba(0,0,0,0.35)] active:transform-[perspective(800px)_rotateX(2deg)_rotateY(-2deg)_translateY(-1px)] transition-all duration-350 ease-out"
              href="https://v.douyin.com/C1hyOBBngI4"
              target="_blank"
            >
              <Icon><Tiktok /></Icon>douyin
            </a>
          </motion.div>
          <motion.div
            :initial="{ opacity: 0, y: 40 }"
            :whileInView="{ opacity: 1, y: 0 }"
            :transition="{ duration: 0.5, delay: 0.6 }"
          >
            <a
              class="btn btn-lg w-36 px-0 font-light text-xl border-transparent bg-[linear-gradient(to_top,transparent_50%,#6e7681_50%)] bg-size-[100%_200%] bg-bottom hover:bg-top hover:transform-[perspective(800px)_rotateX(5deg)_rotateY(-6deg)_translateY(-3px)] hover:[box-shadow:-6px_10px_25px_rgba(0,0,0,0.35)] active:transform-[perspective(800px)_rotateX(2deg)_rotateY(-2deg)_translateY(-1px)] transition-all duration-350 ease-out"
              href="https://github.com/Potatop233"
              target="_blank"
            >
              <Icon><Github /></Icon>Github
            </a>
          </motion.div>
        </div>
      </div>
    </div>

    <footer
      class="footer sm:footer-horizontal bg-gray-700/40 text-base-content p-10"
    >
      <aside class="flex items-center gap-4">
        <img src="/favicon.ico" class="size-20" />
        <div>
          <p class="font-bold text-xl tracking-widest">晨辞の小站</p>
          <p class="text-xs text-gray-400 mt-0.5">
            Built with<br /><b
              >⚪ Vite · Vue · Tailwind · daisyUI · xicons · Motion-v ·
              TypeIt.js</b
            >
          </p>
          <p class="text-xs text-gray-400 mt-3">© 2026 <b>晨辞</b></p>
          <p class="text-xs text-gray-400 mt-1 flex items-center gap-1">
            <Icon><Github /></Icon>
            <a
              class="link link-hover"
              href="https://github.com/Potatop233/chenci_website"
              target="_blank"
              >github.com/Potatop233/chenci_website</a
            >
          </p>
        </div>
      </aside>
      <nav>
        <h6 class="footer-title">友链</h6>
        <a class="link link-hover">敬请期待...</a>
        <a class="link link-hover">敬请期待...</a>
        <a class="link link-hover">敬请期待...</a>
        <a class="link link-hover">敬请期待...</a>
      </nav>
    </footer>
  </div>
</template>

<script lang="ts" setup>
import { motion } from "motion-v";
import { ref, onMounted, onUnmounted, computed } from "vue";
import TypeIt from "typeit";
import { Icon } from "@vicons/utils";
import {
  Qq,
  MailBulk,
  Tiktok,
  Html5,
  Vuejs,
  Google,
  Android,
  Biking,
  PlaneDeparture,
  Camera,
  Xbox,
  Github,
} from "@vicons/fa";
import { AnimalDog16Filled } from "@vicons/fluent";
import { LiveTvOutlined } from "@vicons/material";

let typeitInstance: TypeIt | null = null;
const typeitElement = ref(null);

const Age = computed(() => {
  const birth = new Date(2009, 7, 1);
  const today = new Date();
  let age = today.getFullYear() - birth.getFullYear();
  const monthDiff = today.getMonth() - birth.getMonth();

  if (monthDiff < 0 || (monthDiff === 0 && today.getDate() < birth.getDate())) {
    age--;
  }
  return age;
});

interface Weather {
  province: string;
  city: string;
  district: string;
  weather: string;
  weather_code: number;
  temperature: number;
  feels_like: number;
  visibility: number;
  wind_direction: string;
  wind_power: string;
  humidity: number;
  uv_index: number;
  aqi: number;
  aqi_level: string;
  report_time: string;
}

const weather = ref<Weather | null>(null);
const weatherError = ref(false);

function weatherEmojiFn(code: number) {
  if (code === 100 || code === 150) return "☀️";
  if (code >= 101 && code <= 103) return "⛅";
  if (code >= 151 && code <= 153) return "🌤️";
  if (code === 104 || code === 154) return "☁️";
  if (code >= 300 && code <= 313) return "🌧️";
  if (code >= 400 && code <= 407) return "❄️";
  if (code >= 500 && code <= 502) return "🌫️";
  return "🌈";
}

const weatherEmoji = computed(() => {
  if (!weather.value) return "";
  return weatherEmojiFn(weather.value.weather_code);
});

const copyEmail = () => {
  navigator.clipboard.writeText("1263115878@qq.com");
};

onMounted(async () => {
  try {
    const controller = new AbortController();
    const timeout = setTimeout(() => controller.abort(), 8000);
    const res = await fetch(
      "https://uapis.cn/api/v1/misc/weather?lang=zh&extended=true",
      { signal: controller.signal }
    );
    clearTimeout(timeout);
    const data = await res.json();
    weather.value = {
      ...data,
      feels_like: data.feels_like ?? data.temperature,
      visibility: data.visibility ?? 0,
      aqi: data.aqi ?? 0,
      aqi_level: data.aqi_level ?? "N/A",
      uv_index: data.uv_index ?? 0,
    };
  } catch {
    weather.value = null;
    weatherError.value = true;
  }

  if (typeitElement.value) {
    typeitInstance = new TypeIt(typeitElement.value, {
      speed: 170,
      startDelay: 1000,
      loop: true,
    })
      .type("晨辞- A FURRY", { delay: 2000 })
      .delete()
      .type("一个爱折腾的学生", { delay: 2000 })
      .move(-3)
      .delete(3)
      .type("在努力", { delay: 2000 })
      .move(3)
      .delete(2)
      .type("开发者", { delay: 2000 })
      .delete(3)
      .type("摄影师", { delay: 2000 })
      .delete()
      .go();
  }
});

onUnmounted(() => {
  typeitInstance?.destroy();
});
</script>

