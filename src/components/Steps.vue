<template>  
  <b-container class="steps-container bv-example-row">
    <b-row class="justify-content-md-center">
        <b-col class="breadcrumbs" cols="8" md="auto">
          <ul>
            <li v-on:click="step = 1" :class="classActive(1)">
              <span></span><span>1.</span> Check In
            </li>
            <li v-on:click="step = 2" :class="classActive(2)">
              2. Appointment
            </li>
            <li v-on:click="step = 3" :class="classActive(3)">
              3. Complete
            </li>
          </ul>
        </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {
  name: 'Steps',
  data() {
    return {
      step: 1
    };
  },
  methods: {
    classActive: function(step) {
      return {
        'active-crumb': this.step === step
      };
    }
  },
  computed: {}
};
</script>

<style>
.steps-container {
  margin-top: 40px;
}
.breadcrumbs {
  height: 54px;
}
.breadcrumbs ul {
  display: -ms-flexbox;
  display: flex;
  -ms-flex-direction: row;
  flex-direction: row;
  height: 100%;
  position: relative;
  padding-left: 0;
}
.active-crumb {
  color: rgb(22, 45, 61) !important;
  border-bottom: 2px solid #3899ec !important;
  transition: all 680ms cubic-bezier(0.19, 1, 0.22, 1) 0s !important;
  cursor: default;
}
.breadcrumbs ul li {
  font-size: 12px;
  font-weight: 500;
  display: -ms-flexbox;
  display: flex;
  white-space: nowrap;
  -ms-flex-align: center;
  align-items: center;
  padding: 0 24px;
  text-transform: uppercase;
  /* font-family: "Helvetica65"; */
  letter-spacing: 0.6px;
  position: relative;
  -ms-flex-line-pack: center;
  align-content: center;
  -ms-flex-pack: center;
  justify-content: center;
  color: rgb(122, 146, 165);
  border-bottom: 2px solid rgb(203, 211, 220);
  transition: all 680ms cubic-bezier(0.19, 1, 0.22, 1) 0s;
  cursor: default;
}
.completed-crumb {
}
</style>
