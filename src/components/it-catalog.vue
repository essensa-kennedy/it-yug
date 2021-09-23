<template>
  <div class="container">
    <div class="catalog">
      <it-catalog-item
        v-for="product in products"
        :key="product.id"
        :product_data="product"
        @sendId="showDataFromChild"
      >
      </it-catalog-item>
    </div>
  </div>
</template>

<script>
import itCatalogItem from "./it-catalog-item.vue";

export default {
  name: "it-catalog",
  components: {
    itCatalogItem,
  },
  data() {
    return {
      products: [
        {
          id: 1,
          id_category: 1,
          sale: true,
          img: "000-1",
          title: "Принтер Brother MFC-1123",
          rating: 4.9,
          reviews: 13,
          details: "чёрный А4",
          status: true,
          price: 32999,
        },

        {
          id: 2,
          id_category: 1,
          sale: false,
          img: "000-2",
          title: "Струйный принтер Canon PIXMA G1411",
          rating: 4.2,
          reviews: 2,
          details: "чёрный А4",
          status: true,
          price: 13999,
        },

        {
          id: 3,
          id_category: 1,
          sale: false,
          img: "000-3",
          title: "Лазерный принтер HP LaserJet Pro M404dn (W1A53A)",
          rating: 4.4,
          reviews: 10,
          details: "чёрный А4",
          status: true,
          price: 25999,
        },

        {
          id: 4,
          id_category: 1,
          sale: false,
          img: "000-4",
          title: "Лазерный принтер HP Laser 107a (4ZB77A)",
          rating: 4.9,
          reviews: 26,
          details: "чёрный А4",
          status: true,
          price: 22139,
        },

        {
          id: 5,
          id_category: 1,
          img: "000-5",
          title: "Лазерный принтер Canon i-SENSYS LBP226dw",
          rating: 4.7,
          reviews: 26,
          details: "чёрный А4",
          status: true,
          price: 35999,
        },

        {
          id: 6,
          id_category: 1,
          sale: false,
          img: "000-6",
          title: "Лазерный принтер HP Neverstop Laser 1000w (4RY23A)",
          rating: 4.9,
          reviews: 2,
          details: "чёрный А4",
          status: true,
          price: 32999,
        },
      ],
    };
  },
  methods: {
    showDataFromChild(data) {
      console.log("ID = " + data);
    },
  },
};
</script>
<style lang="scss">
.catalog {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
}
</style>
