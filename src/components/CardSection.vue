v-
<script setup lang="ts"></script>

<template>
  <div
    class="bg-[url('../assets/bg-section-b.png')] bg-no-repeat bg-cover px-40 py-40 flex justify-center items-center w-full"
  >
    <div>
      <h2>For Individuals and Businesses</h2>
      <p>Join 200+ businesses using Eazipay's easy solution.</p>
      <div class="card-stack">
        <div class="card relative" @mouseover="bringToFront(1)">
          <h2>Tamper-proof Payroll for LIfe</h2>
          <p>
            Your staff payroll history is kept in one place forever. No more excel sheet or manual
            records. Download your payroll history anytime you need it.
          </p>
        </div>
        <div class="card left-5" @mouseover="bringToFront(2)">
          <h2>All Payroll, Anytime Anywhere</h2>
          <p>Wherever you are Eazipay has got you covered on ALL your Payroll tasks.</p>
          <p>
            Whether it is Taxes, Pension insurances HMOs, trustfunds, Eazipay handle all your
            compliamces in one place and easily, in seconds!
          </p>
        </div>
        <div class="card absolute left-10" @mouseover="bringToFront(3)">
          <h2>Payroll in Seconds</h2>
          <p>Never again wil you spend more than 2 minutes on payroll.</p>
          <p>Just click on your staff annd bulk-pay them at once.</p>
          <p>Payment is done permanently.</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  data() {},
  methods: {
    bringToFront(cardNumber: any) {
      const cards = document.querySelectorAll('.card')
      cards.forEach((card, index) => {
        const htmlCard = card as HTMLElement
        if (index === cardNumber - 1) {
          htmlCard.style.zIndex = '1'
        } else {
          htmlCard.style.zIndex = '0'
        }
      })
    }
  }
})
</script>

<style scoped>
.card-stack {
  display: flex;
  justify-content: center;
  align-items: flex-end;
  height: 400px;
}

.card {
  width: 300px;
  background-color: #11453b;
  border-radius: 10px;
  box-shadow: 0px 2px 4px rgba(0, 0, 0, 0.1);
  padding: 20px;
  margin: 0 10px;
  color: white;
  transition: z-index 0.3s;
}

.card:hover {
  transform: translateY(-10px);
}
</style>
