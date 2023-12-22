<script>
import Product from "./Product.vue";

export default {
  components: {
    Product,
  },
  data() {
    return {
      products: [
        {
          id: "1",
          imageUrl: "https://3.bp.blogspot.com/-JvNkCMtp_eo/WFNpdTfWIgI/AAAAAAABE3A/Xq3Q0nM5JMUpkLwyQZz8sx7NwAKGypnEwCLcB/s1600/Schaschlik%2BTopf.2.JPG",
          productName: "Keramik Topf",
          productPrice: "19.95 CHF",
          releasedDate: "25.01.2012",
          description: "Idealer Topf für jede Küche. Er würde sorgfälltig aus Porzelan gefertigt und ist sehr robust.",
          rating: 4,
        },
        {
          id: "2",
          imageUrl: "https://img.proidee.at/pimg/1300/21/1300_219389b_0416.jpg",
          productName: "Pannenwender",
          productPrice: "9.95 CHF",
          releasedDate: "17.06.2019",
          description: "Ein sehr robuster Pfannenwender welcher mit einem Glassfasserverstärkenm Griff. Er eignet sich ideal zum",
          rating: 2,
        },
        {
          id: "3",
          imageUrl: "https://th.bing.com/th/id/OIP.bCUt-xzDw3o2psOjJNT92AHaLH?rs=1&pid=ImgDetMain",
          productName: "Kochschürze",
          productPrice: "14.95 CHF",
          releasedDate: "14.02.20.23",
          description: "Diese Kochschürze lest jeden Hobby-Koch richtig cool darstehen. Und sie ist auch noch selbst disingebar",
          rating: 5,
        },
        {
          id: "4",
          imageUrl: "https://th.bing.com/th/id/R.f94186c9e5e3f75ca218bee5910376ae?rik=GtWNroTwQgL%2faw&pid=ImgRaw&r=0",
          productName: "Küchenmesser",
          productPrice: "399.95 CHF",
          releasedDate: "18.10.2017",
          description: "Dieses Handgeschmiedete Küchenmesser wird dein neuer Besterfreund in der Küche werden. Versprochen!",
          rating: 5,
        },
      ],
    };
  },
};
</script>
<template>
  <div v-for="product in products" :key="product.id">
    <Product :data="product" />
  </div>
</template>