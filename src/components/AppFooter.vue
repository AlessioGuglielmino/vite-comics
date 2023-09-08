<script>
export default {
  data() {
    return {
      cards: [
        {
          foto: "buy-comics-digital-comics.png",
          testo: "DIGITAL COMICS",
        },
        {
          foto: "buy-comics-merchandise.png",
          testo: "DC MERCHANDISE",
        },
        {
          foto: "buy-comics-subscriptions.png",
          testo: "SUBSCRIPTION",
        },
        {
          foto: "buy-comics-shop-locator.png",
          testo: "COMIC SHOP LOCATOR",
        },
        {
          foto: "buy-dc-power-visa.svg",
          testo: "DC POWER VISA",
        },
      ],

      dcComics: [
        "Characters",
        "Comics",
        "Movies",
        "Tv",
        "Games",
        "Videos",
        "News",
      ],
      Shops: ["Shop DC", "Shop DC Collectibles"],
      dc: [
        "Term of use",
        "Privacy policy",
        "Ad choice",
        "Adversing",
        "Jobs",
        "Subscriptions ",
        "Talent",
        "CPSC Certificates",
        "Rating",
        "Show help",
        "Contact us",
      ],
      sites: [
        " DC",
        "MAD Magazine",
        " DC Kids",
        " DC Universe",
        " DC Power Visa",
      ],
    };
  },
};
</script>

<template>
  <footer>
    <!-- TOP FOOTER  -->
    <div class="top">
      <ul>
        <li v-for="card in cards">
          <img :src="'./img/' + card.foto" alt="" /> {{ card.testo }}
        </li>
      </ul>
    </div>

    <!-- CENTER FOOTER  -->
    <div class="center">
      <div class="left">
        <div>
          <ul>
            <h4>DC COMICS</h4>
            <li v-for="option in dcComics">{{ option }}</li>
          </ul>
          <ul>
            <h4>SHOP</h4>
            <li v-for="shop in Shops">{{ shop }}</li>
          </ul>
        </div>
        <ul>
          <h4>DC</h4>
          <li v-for="option in dc">{{ option }}</li>
        </ul>
        <ul>
          <h4>SITES</h4>
          <li v-for="option in sites">{{ option }}</li>
        </ul>
      </div>
      <div class="right"></div>
    </div>

    <!-- BOTTOM FOOTER  -->
    <div class="bottom"></div>
  </footer>
</template>

<style lang="scss" scoped>
.top {
  background-color: #0282f9;
  height: 150px;
  display: flex;
  justify-content: space-around;

  ul {
    display: flex;
    list-style: none;
    gap: 3rem;
  }

  li {
    display: flex;
    align-items: center;
    gap: 0.7rem;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 0.7rem;
    font-weight: bold;
  }
  img {
    width: 50px;
  }
}

.center {
  background-image: url("../../public/img/footer-bg.jpg");
  height: 300px;
  color: rgb(174, 167, 167);

  .left {
    height: 100%;
    display: flex;
    gap: 2rem;
    margin: 0 15%;
  }

  h4 {
    color: rgb(238, 230, 230);
    font-weight: bolder;
    padding-top: 10px;
  }

  li {
    margin-top: 5px;
    list-style: none;
  }
}
</style>
