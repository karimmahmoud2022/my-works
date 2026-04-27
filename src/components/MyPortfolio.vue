<template>
  <div class="hero">
    <div class="container">
      <div class="row pt-5">
        <div class="col-sm-6 col-12">
          <div class="content">
            <div class="hero-tag d-flex gap-2 align-items-center">
              <span></span>
              كريم محمود ابراهيم عطية
            </div>
            <h1>
              مطور <br />
              <span>vue.js</span> <br />
              و wordpress
            </h1>
            <p>
              أبني واجهات سريعة ومتجاوبة بـ <span>Vue.js</span>، <br />
              وأطوّر مواقع احترافية بـ <span>WordPress</span> من التصميم للإطلاق.
            </p>
            <div
              class="technology d-flex justify-content-start gap-4 mt-5 align-items-center"
            >
              <div
                class="vue d-flex align-items-center gap-2 p-1 px-3 text-white fw-bold"
              >
                <span></span>
                Vue.js
              </div>
              <div
                class="wordPress d-flex align-items-center gap-2 p-1 px-3 text-white fw-bold"
              >
                <span></span>
                WordPress
              </div>
              <div
                class="wooCommerce d-flex align-items-center gap-2 p-1 px-3 text-white fw-bold"
              >
                <span></span>
                WooCommerce
              </div>
            </div>
            <div
              class="button-action d-flex justify-content-start mt-5 gap-5 align-content-center"
            >
              <div class="btn btn-lights rounded-5 p-3">استعراض اعمالي</div>
              <div class="btn btn-light rounded-5 p-3">تواصل معي</div>
            </div>
          </div>
        </div>
        <div class="col-sm-6 col-12 mt-5">
          <div class="hero-right bg-dark rounded">
            <div class="code-card">
              <div class="code-bar">
                <div class="dot" style="background: #ff5f57"></div>
                <div class="dot" style="background: #febc2e"></div>
                <div class="dot" style="background: #28c840"></div>
                <span class="fname">App.vue</span>
              </div>
              <div class="code-body">
                <div><span class="cm">// مرحباً بك ✦</span></div>
                <div>&nbsp;</div>
                <div><span class="cp">const</span> <span class="cb">dev</span> = {</div>
                <div>
                  &nbsp;&nbsp;<span class="cg">name</span>:
                  <span class="cy">' karim mahmoud'</span>,
                </div>
                <div>&nbsp;&nbsp;<span class="cg">stack</span>: [</div>
                <div>&nbsp;&nbsp;&nbsp;&nbsp;<span class="cy">'Vue.js 3'</span>,</div>
                <div>&nbsp;&nbsp;&nbsp;&nbsp;<span class="cy">'WordPress'</span>,</div>
                <div>&nbsp;&nbsp;&nbsp;&nbsp;<span class="cy">'Nuxt.js'</span>,</div>
                <div>&nbsp;&nbsp;],</div>
                <div>
                  &nbsp;&nbsp;<span class="cg">available</span>:
                  <span class="cp">true</span>,
                </div>
                <div>}</div>
                <div>&nbsp;</div>
                <div>
                  <span class="cp">export default</span> <span class="cb">dev</span>
                </div>
              </div>
            </div>

            <div class="stats-row">
              <div class="stat-box" v-for="s in stats" :key="s.l">
                <span class="sn">{{ s.n }}</span>
                <span class="sl">{{ s.l }}</span>
              </div>
            </div>
          </div>
          <div
            class="hero-conuter mt-4 d-flex justify-content-center align-items-center gap-3"
          >
            <div class="counter rounded shadow p-3 text-center bg-dark text-white">
              <div class="number">80+</div>
              <div class="labal">مشروع</div>
            </div>
            <div class="counter rounded shadow p-3 text-center bg-dark text-white">
              <div class="number">20+</div>
              <div class="labal">عميل</div>
            </div>
            <div class="counter rounded shadow p-3 text-center bg-dark text-white">
              <div class="number">5+</div>
              <div class="labal">سنوات</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.hero {
  background-image: linear-gradient(rgba(255, 255, 255, 0.07) 1px, transparent 1px),
    linear-gradient(90deg, rgba(255, 255, 255, 0.07) 1px, transparent 1px);
  background-size: 72px 72px;
  height: 100vh;
  width: 100%;

  display: flex;
  align-items: center;
}
.hero-tag {
  padding: 6px 16px;
  background-color: #42d3921a;
  border: 2px solid #42d39237;
  border-radius: 25px;
  width: fit-content;
}
.hero-tag {
  font-size: 13px;
  font-weight: 700;
  color: #fff;
}
.hero-tag span {
  display: inline-block;
  background-color: #42d392;
  width: 6px !important;
  height: 6px !important;
  border-radius: 50%;
  animation: identifier 2s infinite;
}

@keyframes identifier {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}

.content h1 {
  font-size: 70px !important;
  color: #fff;
  font-weight: 900;
}

.content h1 span {
  color: #42d392;
}
.content p {
  color: #bcbcbc;
  font-size: 18px;
}
.content p span {
  color: #fff;
  font-weight: 900;
}
.technology .vue,
.wordPress,
.wooCommerce {
  background-color: #42d3921a;
  border: 2px solid #42d39237;
  border-radius: 25px;
  width: fit-content;
}
.technology span {
  width: 6px;
  height: 6px;
  border-radius: 50%;
  background-color: #42d392;
  animation: identifier 2s infinite;
}
.btn-light {
  background-color: #42d39200 !important;
  color: #fff;
  font-weight: 500;
  border: 1px solid #42d392;
}
.btn-lights:hover {
  background-color: #42d39200 !important;
  color: #fff;
  border: 1px solid #42d392;
}
.btn-light:hover {
  background-color: #42d392 !important;
  color: #fff;
  border: 1px solid #42d392;
}
.btn-lights {
  background-color: #42d392 !important;
  color: #fff;
  font-weight: 500;
  border: 1px solid #42d392;
}

.hero-right {
  position: relative;
  z-index: 1;
  display: flex;
  flex-direction: column;
  gap: 1.2rem;
}
.code-card {
  background: var(--ink);
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 28px 70px rgba(15, 14, 11, 0.2);
  animation: float 4s ease-in-out infinite;
}
.code-card:hover {
  animation: none;
  transform: rotate(0) !important;
}
@keyframes float {
  0%,
  100% {
    transform: rotate(2deg) translateY(0);
  }
  50% {
    transform: rotate(2deg) translateY(-10px);
  }
}
.code-bar {
  background: #1a1917;
  padding: 0.7rem 1rem;
  display: flex;
  align-items: center;
  gap: 0.45rem;
}
.dot {
  width: 10px;
  height: 10px;
  border-radius: 50%;
}
.fname {
  font-size: 0.65rem;
  color: #5a5854;
  margin-right: auto;
}
.code-body {
  padding: 1.4rem 1.8rem;
  font-size: 0.76rem;
  line-height: 2;
  color: #c0bcb4;
}
.cg {
  color: #42b883;
}
.cb {
  color: #7ec8e3;
}
.cy {
  color: #f6d860;
}
.cp {
  color: #ff7eb3;
}
.cm {
  color: #5a5854;
}
</style>

