<template>
  <h1>Full Name : {{ fullName }}</h1>
</template>
<script>
export default {
  data() {
    return {
      firstName: "JeongWoo",
      lastName: "Cho",
      fullName: "",
    };
  },
  watch: {
    firstName() {
      this.fullName = this.firstName + " " + this.lastName;
    },
    lastName() {
      this.fullName = this.firstName + " " + this.lastName;
    },
  },
};
</script>
