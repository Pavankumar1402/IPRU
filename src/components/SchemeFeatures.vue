<template>
  <section class="default-section">
    <div class="container">
      <h1 class="text-light-blue">Scheme Features</h1>
      <div class="row" v-for="(data, i) in SchemeFeatures" :key="i">
        <div class="col-4 p-3 border-end border-bottom">
          <span class="text-light-blue fw-600 fs-18 ">
            {{ data.name }}
          </span>
        </div>
        <div class="col-8 p-3 border-bottom">
          <p>
            {{ data.description }}
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      SchemeFeatures: [
        {
          name: "Type of Scheme",
          description:
            "An open ended equity scheme predominantly investing in large cap stocks",
        },
        {
          name: "Plans",
          description:
            "Growth & IDCW(IDCW payout*** and re-investment facility available)",
        },
        {
          name: "Min. Application Amount",
          description: "Rs.100 (plus in multiples of Re.1)",
        },
        {
          name: "Min. Additional Investment",
          description: "Rs.100 (plus in multiples of Re.1)",
        },
        {
          name: "Minimum Redemption Amt.",
          description: "Any Amount",
        },
        {
          name: "Entry Load",
          description: "Not Applicable.",
        },
        {
          name: "Exit Load",
          description:
            "Upto 1 Year from allotment 1% of applicable NAV,more than 1 Year Nil",
        },
        {
          name: "Fund Manager",
          description:
            " Anish Tawakley {Managing this fund since Sep, 2018 & Overall 26 years of experience}Rajat Chandak {Managing this fund since Jul, 2017 & Overall 11 years of experience}Vaibhav Dusad {Managing this fund since Jan, 2021 & Overall 9 years of experience} #",
        },
      ],
    };
  },
};
</script>

<style></style>
