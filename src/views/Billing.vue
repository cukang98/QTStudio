<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-lg-12">
        <div class="row mt-4">
          <div class="col-md-12 mb-4">
            <ProductCategoryCard />
          </div>
        </div>
      </div>

    </div>
    <div class="row">
      <div class="col-md-7">
        <billing-card />
      </div>
      <div class="col-md-5">
        <transaction-card />
      </div>
    </div>
  </div>
</template>

<script>
//import MasterCard from "@/examples/Cards/MasterCard.vue";
//import DefaultInfoCard from "@/examples/Cards/DefaultInfoCard.vue";
import ProductCategoryCard from "./components/ProductCategoryCard.vue";
//import InvoiceCard from "./components/InvoiceCard.vue";
import BillingCard from "./components/BillingCard.vue";
import TransactionCard from "./components/TransactionCard.vue";

export default {
  name: "Product",
  components: {
    //MasterCard,
    //DefaultInfoCard,
    ProductCategoryCard,
    //InvoiceCard,
    BillingCard,
    TransactionCard,
  },
  data() {
    return {
      salary: {
        classIcon: "text-white fas fa-landmark",
        title: "Salary",
        desc: "Belong Interactive",
        price: "+$2000",
      },
      paypal: {
        classIcon: "text-white fab fa-paypal",
        title: "Paypal",
        desc: "Freelance Payment",
        price: "$455.00",
      },
    };
  },
};
</script>
