<template>
  <div class="home">
    <h1>Fuel Manager</h1>
    <h2>Total amount of money spent, grouped by month</h2>
    <select id="chooseMonth" @change="selectMonth($event)">
      <option value="0">Choose Month</option>
      <option value="1">Jan</option>
      <option value="2">Feb</option>
      <option value="3">March</option>
      <option value="4">April</option>
      <option value="5">May</option>
      <option value="6">June</option>
      <option value="7">July</option>
      <option value="8">August</option>
      <option value="9">September</option>
      <option value="10">October</option>
      <option value="11">November</option>
      <option value="12">December</option>
    </select>

    <input type="text" disabled v-model="monthlyCosts">
  </div>
</template>

<script>
import $ from "jquery";
export default {
  name: "Home", //this is the name of the component
  data: function() {
    return {
      monthlyCosts: 0
    };
  },

  methods: {
    selectMonth: function(event) {
      const month = event.target.value;
      let that = this;
      $.get("http://localhost:8080/Fuels/" + month, function(data) {
        that.monthlyCosts = data[0].total;
      });
    },
    selectMonthByDriver: function(event) {
      const driver = event.target.value;
      let that = this;
      $.get("http://localhost:8080/Fuels/" + month, function(data) {
        that.monthlyCosts = data[0].total;
      });
    }
  }
};
</script>
<style>
p {
  text-align: center;
}
</style>