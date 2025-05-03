<template>
  <div class="flex items-center justify-center h-screen bg-[#DAF0FF]">
    <div class="bg-white w-[375px] h-[812px] p-6 rounded-3xl shadow-lg flex flex-col justify-between">
      <div>
        <div class="text-gray-400 text-3xl mb-1 text-right h-1/5">{{ expression }}</div>
        <div class="text-5xl font-bold text-black mb-4 text-right h-1/3 align-middle">= {{ result }}</div>
      </div>
      <div class="grid grid-cols-4 gap-2">
        <button class="btn-func" @click="clear">Ac</button>
        <button class="btn-func" disabled>e</button>
        <button class="btn-func" disabled>μ</button>
        <button class="btn-func" disabled>sin</button>
        <button class="btn-num" @click="append('7')">7</button>
        <button class="btn-num" @click="append('8')">8</button>
        <button class="btn-num" @click="append('9')">9</button>
        <button class="btn-op" @click="append('-')">-</button>
        <button class="btn-num" @click="append('4')">4</button>
        <button class="btn-num" @click="append('5')">5</button>
        <button class="btn-num" @click="append('6')">6</button>
        <button class="btn-op" @click="append('+')">+</button>
        <button class="btn-num" @click="append('1')">1</button>
        <button class="btn-num" @click="append('2')">2</button>
        <button class="btn-num" @click="append('3')">3</button>
        <button class="btn-op" @click="append('*')">*</button>
        <button class="btn-num" @click="append('0')">0</button>
        <button class="btn-func" disabled>deg</button>
        <button class="btn-op" @click="append('/')">/</button>
        <button class="btn-equal" @click="calculate">=</button>
      </div>
      
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue';

const expression = ref('');
const result = ref('');

const append = (val) => {
  expression.value += val;
};

const clear = () => {
  expression.value = '';
  result.value = '';
};

const calculate = () => {
  try {
    // Basic eval alternative (CAUTION: eval should not be used in production apps)
    result.value = eval(expression.value);
  } catch {
    result.value = 'Error';
  }
};
</script>

<style scoped>
.btn-num,
.btn-func,
.btn-op,
.btn-equal {
  @apply bg-white text-sky-500 font-semibold py-2 rounded-xl shadow-sm h-[60px] w-[62px];
}
.btn-num:hover,
.btn-func:hover,
.btn-op:hover {
  @apply bg-blue-50;
}
.btn-equal {
  @apply bg-blue-500 text-white font-bold;
}
</style>
