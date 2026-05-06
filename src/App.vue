<template>
  <div class="app">

    <h1>L3SODB Timetable 26</h1>

    <!-- Monday -->
    <div class="day-box">
      <div class="day-header" @click="toggleDay('Mo')">
        <span>Monday</span>
        <span>{{ openDay === 'Mo' ? '▲' : '▼' }}</span>
      </div>
      <div v-if="openDay === 'Mo'" class="lessons">
        <div class="lesson"><span class="period-info">Period 1 | 8:00-8:40</span><span class="subject">UI/UX</span><span class="teacher">Teacher: MAC</span></div>
        <div class="lesson"><span class="period-info">Period 2 | 8:40-9:20</span><span class="subject">UI/UX</span><span class="teacher">Teacher: MAC</span></div>
        <div class="lesson"><span class="period-info">Period 3 | 9:20-10:00</span><span class="subject">UI/UX</span><span class="teacher">Teacher: MAC</span></div>
        <div class="break">--- BREAK ---</div>
        <div class="lesson"><span class="period-info">Period 4 | 10:20-11:00</span><span class="subject">DJF</span><span class="teacher">Teacher: UT</span></div>
        <div class="lesson"><span class="period-info">Period 5 | 11:00-11:40</span><span class="subject">Free</span></div>
        <div class="lesson"><span class="period-info">Period 6 | 11:40-12:20</span><span class="subject">Free</span></div>
        <div class="break">--- LUNCH ---</div>
        <div class="lesson"><span class="period-info">Period 7 | 13:00-13:40</span><span class="subject">MATH</span><span class="teacher">Teacher: IA</span></div>
        <div class="lesson"><span class="period-info">Period 8 | 13:40-14:20</span><span class="subject">MATH</span><span class="teacher">Teacher: IA</span></div>
        <div class="break">--- BREAK ---</div>
        <div class="lesson"><span class="period-info">Period 9 | 14:40-15:20</span><span class="subject">GD</span><span class="teacher">Teacher: RJA</span></div>
        <div class="lesson"><span class="period-info">Period 10 | 15:20-16:00</span><span class="subject">Free</span></div>
      </div>
    </div>

    <!-- Tuesday -->
    <div class="day-box">
      <div class="day-header" @click="toggleDay('Tu')">
        <span>Tuesday</span>
        <span>{{ openDay === 'Tu' ? '▲' : '▼' }}</span>
      </div>
      <div v-if="openDay === 'Tu'" class="lessons">
        <div class="lesson"><span class="period-info">Period 1 | 8:00-8:40</span><span class="subject">DJF</span><span class="teacher">Teacher: UT</span></div>
        <div class="lesson"><span class="period-info">Period 2 | 8:40-9:20</span><span class="subject">DJF</span><span class="teacher">Teacher: UT</span></div>
        <div class="lesson"><span class="period-info">Period 3 | 9:20-10:00</span><span class="subject">DJF</span><span class="teacher">Teacher: UT</span></div>
        <div class="break">--- BREAK ---</div>
        <div class="lesson"><span class="period-info">Period 4 | 10:20-11:00</span><span class="subject">DJF Pract</span><span class="teacher">Teacher: UT</span></div>
        <div class="lesson"><span class="period-info">Period 5 | 11:00-11:40</span><span class="subject">DJF Pract</span><span class="teacher">Teacher: UT</span></div>
        <div class="lesson"><span class="period-info">Period 6 | 11:40-12:20</span><span class="subject">DJF Pract</span><span class="teacher">Teacher: UT</span></div>
        <div class="break">--- LUNCH ---</div>
        <div class="lesson"><span class="period-info">Period 7 | 13:00-13:40</span><span class="subject">CL</span><span class="teacher">Teacher: SU</span></div>
        <div class="lesson"><span class="period-info">Period 8 | 13:40-14:20</span><span class="subject">CL</span><span class="teacher">Teacher: SU</span></div>
        <div class="break">--- BREAK ---</div>
        <div class="lesson"><span class="period-info">Period 9 | 14:40-15:20</span><span class="subject">VC Pract</span><span class="teacher">Teacher: IS</span></div>
        <div class="lesson"><span class="period-info">Period 10 | 15:20-16:00</span><span class="subject">Free</span></div>
      </div>
    </div>

    <!-- Wednesday -->
    <div class="day-box">
      <div class="day-header" @click="toggleDay('We')">
        <span>Wednesday</span>
        <span>{{ openDay === 'We' ? '▲' : '▼' }}</span>
      </div>
      <div v-if="openDay === 'We'" class="lessons">
        <div class="lesson"><span class="period-info">Period 1 | 8:00-8:40</span><span class="subject">VC</span><span class="teacher">Teacher: IG</span></div>
        <div class="lesson"><span class="period-info">Period 2 | 8:40-9:20</span><span class="subject">VC</span><span class="teacher">Teacher: IG</span></div>
        <div class="lesson"><span class="period-info">Period 3 | 9:20-10:00</span><span class="subject">VC</span><span class="teacher">Teacher: IG</span></div>
        <div class="break">--- BREAK ---</div>
        <div class="lesson"><span class="period-info">Period 4 | 10:20-11:00</span><span class="subject">DGV</span><span class="teacher">Teacher: MS</span></div>
        <div class="lesson"><span class="period-info">Period 5 | 11:00-11:40</span><span class="subject">DGV</span><span class="teacher">Teacher: MS</span></div>
        <div class="lesson"><span class="period-info">Period 6 | 11:40-12:20</span><span class="subject">DGV</span><span class="teacher">Teacher: MS</span></div>
        <div class="break">--- LUNCH ---</div>
        <div class="lesson"><span class="period-info">Period 7 | 13:00-13:40</span><span class="subject">Free</span></div>
        <div class="lesson"><span class="period-info">Period 8 | 13:40-14:20</span><span class="subject">Free</span></div>
        <div class="break">--- BREAK ---</div>
        <div class="lesson"><span class="period-info">Period 9 | 14:40-15:20</span><span class="subject">MATH</span><span class="teacher">Teacher: K IA</span></div>
        <div class="lesson"><span class="period-info">Period 10 | 15:20-16:00</span><span class="subject">Free</span></div>
      </div>
    </div>

    <!-- Thursday -->
    <div class="day-box">
      <div class="day-header" @click="toggleDay('Th')">
        <span>Thursday</span>
        <span>{{ openDay === 'Th' ? '▲' : '▼' }}</span>
      </div>
      <div v-if="openDay === 'Th'" class="lessons">
        <div class="lesson"><span class="period-info">Period 1 | 8:00-8:40</span><span class="subject">UI/UX</span><span class="teacher">Teacher: MAC</span></div>
        <div class="lesson"><span class="period-info">Period 2 | 8:40-9:20</span><span class="subject">UI/UX</span><span class="teacher">Teacher: MAC</span></div>
        <div class="lesson"><span class="period-info">Period 3 | 9:20-10:00</span><span class="subject">UI/UX</span><span class="teacher">Teacher: MAC</span></div>
        <div class="break">--- BREAK ---</div>
        <div class="lesson"><span class="period-info">Period 4 | 10:20-11:00</span><span class="subject">DJF</span><span class="teacher">Teacher: UT</span></div>
        <div class="lesson"><span class="period-info">Period 5 | 11:00-11:40</span><span class="subject">DJF Pract</span><span class="teacher">Teacher: UT</span></div>
        <div class="lesson"><span class="period-info">Period 6 | 11:40-12:20</span><span class="subject">Free</span></div>
        <div class="break">--- LUNCH ---</div>
        <div class="lesson"><span class="period-info">Period 7 | 13:00-13:40</span><span class="subject">PHY</span><span class="teacher">Teacher: MI</span></div>
        <div class="lesson"><span class="period-info">Period 8 | 13:40-14:20</span><span class="subject">PHY</span><span class="teacher">Teacher: MI</span></div>
        <div class="break">--- BREAK ---</div>
        <div class="lesson"><span class="period-info">Period 9 | 14:40-15:20</span><span class="subject">DJF Pract</span><span class="teacher">Teacher: UT</span></div>
        <div class="lesson"><span class="period-info">Period 10 | 15:20-16:00</span><span class="subject">DJF Pract</span><span class="teacher">Teacher: UT</span></div>
      </div>
    </div>

    <!-- Friday -->
    <div class="day-box">
      <div class="day-header" @click="toggleDay('Fr')">
        <span>Friday</span>
        <span>{{ openDay === 'Fr' ? '▲' : '▼' }}</span>
      </div>
      <div v-if="openDay === 'Fr'" class="lessons">
        <div class="lesson"><span class="period-info">Period 1 | 8:00-8:40</span><span class="subject">DGV</span><span class="teacher">Teacher: MIS</span></div>
        <div class="lesson"><span class="period-info">Period 2 | 8:40-9:20</span><span class="subject">DGV</span><span class="teacher">Teacher: MIS</span></div>
        <div class="lesson"><span class="period-info">Period 3 | 9:20-10:00</span><span class="subject">DGV</span><span class="teacher">Teacher: MIS</span></div>
        <div class="break">--- BREAK ---</div>
        <div class="lesson"><span class="period-info">Period 4 | 10:20-11:00</span><span class="subject">FR</span><span class="teacher">Teacher: MIS</span></div>
        <div class="lesson"><span class="period-info">Period 5 | 11:00-11:40</span><span class="subject">Free</span></div>
        <div class="lesson"><span class="period-info">Period 6 | 11:40-12:20</span><span class="subject">Free</span></div>
        <div class="break">--- LUNCH ---</div>
        <div class="lesson"><span class="period-info">Period 7 | 13:00-13:40</span><span class="subject">Free</span></div>
        <div class="lesson"><span class="period-info">Period 8 | 13:40-14:20</span><span class="subject">Free</span></div>
        <div class="break">--- BREAK ---</div>
        <div class="lesson"><span class="period-info">Period 9 | 14:40-15:20</span><span class="subject">Free</span></div>
        <div class="lesson"><span class="period-info">Period 10 | 15:20-16:00</span><span class="subject">Free</span></div>
      </div>
    </div>

  </div>
</template>

<script setup>
import { ref } from 'vue'

// null means nothing is open at the start
const openDay = ref(null)

// clicking same day closes it, clicking a new day opens it
function toggleDay(day) {
  if (openDay.value === day) {
    openDay.value = null
  } else {
    openDay.value = day
  }
}
</script>

<style scoped>
.app {
  max-width: 500px;
  margin: 0 auto;
  padding: 20px;
  font-family: Arial, sans-serif;
  background: #f2f2f2;
  min-height: 100vh;
}

h1 {
  text-align: center;
  color: #111111;
  margin-bottom: 24px;
}

/* each day box */
.day-box {
  border: 1px solid #cccccc;
  border-radius: 8px;
  margin-bottom: 10px;
  overflow: hidden;
}

/* clickable header */
.day-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 14px 18px;
  background: #222222;
  color: #ffffff;
  cursor: pointer;
  font-size: 16px;
  font-weight: 500;
}

.day-header:hover {
  background: #444444;
}

/* lessons container */
.lessons {
  padding: 10px 14px;
  background: #ffffff;
}

/* each lesson row */
.lesson {
  background: #f9f9f9;
  border-left: 4px solid #555555;
  padding: 10px 14px;
  margin-bottom: 6px;
  border-radius: 0 4px 4px 0;
  display: flex;
  flex-direction: column;
  gap: 2px;
}

.period-info {
  font-size: 11px;
  color: #999999;
}

.subject {
  font-size: 15px;
  font-weight: 500;
  color: #111111;
}

.teacher {
  font-size: 12px;
  color: #555555;
}

/* break and lunch */
.break {
  text-align: center;
  color: #999999;
  font-size: 12px;
  margin: 8px 0;
}
</style>