<template>
  <div>
    <slots-example>
      <template v-slot:companyName>
        <div><b>Company Name:</b> Elves LLC</div>
      </template>
      <template v-slot:addressLine1>
        <div><b>Address Line 1:</b> 123 Road NorthPole</div>
      </template>
      <template v-slot:city>
        <div><b>City:</b> North Pole</div>
      </template>
      <template v-slot:state>
        <div><b>State:</b> Alaska</div>
      </template>
      <template v-slot:country>
        <div><b>Country:</b> United States</div>
      </template>
      <template v-slot:postalCode>
        <div><b>Postal Code:</b> 12345</div>
      </template>
    </slots-example>
  </div>
</template>

<script>
import SlotsExample from './components/SlotsExample.vue';

export default {
  components: { SlotsExample },
  name: 'App',
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
