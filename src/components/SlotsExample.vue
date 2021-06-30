<template>
  <div>
    <slot v-for="slotName in slotNames" :key="slotName" :name="slotName" />
  </div>
</template>

<script>
export default {
  name: 'SlotsExample',
  data() {
    return {
      slotNames: [
        'companyName',
        'addressLine1',
        'city',
        'state',
        'country',
        'postalCode',
      ],
    };
  },
  created() {
    this.slotNames = this.shuffle(this.slotNames);
  },
  methods: {
    // This is to simulate randomization of some format
    // that could be passed in to this component as a `prop`
    shuffle(array) {
      let currentIndex = array.length;
      let temporaryValue;
      let randomIndex;

      // While there remain elements to shuffle...
      while (0 !== currentIndex) {
        // Pick a remaining element...
        randomIndex = Math.floor(Math.random() * currentIndex);
        currentIndex -= 1;

        // And swap it with the current element.
        temporaryValue = array[currentIndex];
        array[currentIndex] = array[randomIndex];
        array[randomIndex] = temporaryValue;
      }

      return array;
    },
  },
};
</script>
