<template>
  <v-row id="row">
    <v-col id="teix" class="d-flex child-flex kolon" cols="12" sm="12">
      <v-card>
        <Car2 id="karosel"></Car2>
      </v-card>
    </v-col>

    <v-col id="ggg" class="d-flex child-flex kolon" sm="12" cols="12" style="padding:0px">
      <v-card>
        <v-img
          :src="`https://www.camper.com/cms/api/assets/tiers-banners-homes/cf40e2b2-c2ac-47e0-99d7-750b0c01c3a7/T93-W45-GIFT-DIST_Desktop.avif={}`"
          aspect-ratio="2"
          class="images"
        >
          <div style="margin-left:-250px">
              <div id="itemsdiv2">
                <span class="giffspan">Gift Guide<br /> </span>
                <span class="lilspan"> En Mükemmel Hediyeyi Bulun<br /> </span>
              </div>
              <div style="display:flex; margin-top:20px; margin-left:30px;" >
                <v-btn
                  to="/gift"
                  class="butonlar"
                  id="btn7"
                  >Kadın</v-btn
                ><v-btn
                  to="/gift"
                  class="butonlar"
                  id="btn8"
                  >Erkek</v-btn
                ><v-btn
                  to="/gift"
                  class="butonlar"
                  id="btn9"
                  >Çocuk</v-btn
                >
              </div>
          </div>
        </v-img>
      </v-card>
    </v-col>

    <v-col class="d-flex child-flex kolon" cols="12" sm="12">
      <v-card>
        <v-img
          src="https://www.camper.com/cms/api/assets/tiers-banners-homes/2567a1e8-f454-4813-8004-31475bb67315/T93-MSS-noproduct-Desktop.avif"
          aspect-ratio="2"
          class="images"
        >
          <v-text class="sez"> Sezon Ortası İndirimi </v-text>
          <v-spacer></v-spacer>
          <v-text class="gifspan">%30'a Varan İndirim<br /> </v-text>
          <v-btn id="btnKadın" class="butonlar" depressed to="/kadın"> Kadın </v-btn>
          <v-btn id="btnErkek" class="butonlar" depressed to="/erkek"> Erkek </v-btn>
        </v-img>
      </v-card>
    </v-col>

    <v-col class="d-flex child-flex kolon" cols="12" sm="12">
      <v-card>
        <Carousel id="karosel"></Carousel>
      </v-card>
    </v-col>

    <v-col id="ewew" class="d-flex child-flex kolon" cols="12" sm="12">
      <v-card>
        <v-img src="@/assets/camper_gif.gif" aspect-ratio="2" class="images">
          <v-text class="sez"> 11. Sayı Kıbrıs </v-text>
          <v-spacer></v-spacer>
          <v-text class="gifspan">The Walking Society<br /> </v-text>
          <v-spacer></v-spacer>
          <v-btn id="kampanya" class="butonlar" depressed> Kampanyaya Göz Atın </v-btn>
        </v-img>
      </v-card>
    </v-col>

    <v-col class="d-flex child-flex kolon" sm="12" cols="12">
      <v-card>
        <v-img
          :src="`https://www.camper.com/cms/api/assets/tiers-banners-homes/22fa517d-a949-4119-a210-cbb08370536a/T93_Peu-Stedium_2000x1125_desktop.avif={}`"
          aspect-ratio="2"
          class="images"
        >
          <div class="itemsdiv">
            <span class="giffspan"> Peu Stadium<br /> </span>
            <span class="lilspan"> Koleksiyonu Keşfet<br /> </span>
            <v-btn depressed elevation="2" floating class="butonlar" id="btn2"
              >Daha Fazlası</v-btn
            >
          </div>
        </v-img>
      </v-card>
    </v-col>

    <v-col class="d-flex child-flex kolon" cols="6">
      <v-card>
        <v-img
          :src="`https://www.camper.com/cms/api/assets/tiers-banners-homes/2429b0c7-0187-4d37-b5e4-ef9d3293b1ae/T93-Gender-Walden-Women-desktop.avif={}`"
          aspect-ratio="1"
          class="images"
        >
          <v-btn
            depressed
            elevation="2"
            floating
            class="butonlar"
            id="btn3"
            to="/kadın"
            >Kadın</v-btn
          >
        </v-img>
      </v-card>
    </v-col>

    <v-col class="d-flex child-flex kolon" cols="6">
      <v-img
        :src="`https://www.camper.com/cms/api/assets/tiers-banners-homes/7cf1e10a-0c2f-4505-9835-c52f97182916/T93-Gender-Walden-Men-desktop.avif={}`"
        aspect-ratio="1"
        class="images"
      >
        <v-btn
          depressed
          elevation="2"
          floating
          class="butonlar"
          id="btn4"
          to="/erkek"
          >Erkek</v-btn
        >
      </v-img>
    </v-col>

    <v-col class="d-flex child-flex kolon" cols="12">
      <v-img
        :src="`https://www.camper.com/cms/api/assets/tiers-banners-homes/c565ea73-9386-4b44-bd51-8389176cde27/T93_Store-locator-Dist-desktop.avif={}`"
        aspect-ratio="2"
        class="images"
      >
        <v-btn
          depressed
          elevation="2"
          floating
          class="butonlar"
          id="btn5"
          to="/magaza"
          >En Yakın Mağazayı Bul</v-btn
        >
      </v-img>
    </v-col>
  </v-row>
</template>

<style scoped >
#karosel {
  aspect-ratio: 1.8;
}

.kolon {
  padding: 0px;
}
#row {
  z-index: 0;
}

#ewew {
  margin-top: -295px;
}
#text {
  padding-left: 650px;
}

#maindiv {
  font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Oxygen,
    Ubuntu, Cantarell, Fira Sans, Droid Sans, Helvetica Neue, sans-serif;
}

.lilspan {
  color: white;
  font-size: 30px;
  margin-left: -500px;
}
#itemsdiv2 {
  text-align: center;
}
#ggg {
  margin-top: -275px;
}
.peuspan {
  color: white;
  font-size: 70px;
  margin-right: 600px;
}

.sez {
  color: white;
  font-size: 50px;
  margin-right: 500px;
}
.gifspan {
  color: white;
  font-size: 70px;
  margin-right: 850px;
}
.giffspan {
  color: white;
  font-size: 70px;
  margin-left: -500px;
}
.colspan {
  color: white;
  font-size: 30px;
  margin-right: 600px;
}

.images {
  text-align: center;
  align-items: center;
  margin: auto;
  object-position: center;
}

.butonlar {
  text-transform: none;
  position: relative;
  border-radius: 0px;
}

.itemsdiv {
  margin: auto;
}

#btn1:hover,
#btn2:hover,
#btn3:hover,
#btn4:hover,
#btn5:hover {
  background-color: black;
  color: white;
}

.butonlar:hover{
  background-color: black;
  color: white;
}

#btn1 {
  margin-top: 20px;
  margin-right: 520px;
}
#btn2 {
  margin-top: 20px;
  margin-right: 600px;
}
#btn3 {
  margin-right: 350px;
}
#btn4 {
  margin-right: 300px;
}
#btn5 {
  margin-right: 650px;
}
#btn7 {
  width: 150px;
  border-radius: 0;
  text-transform: none;
  height: 40px;
  transition: 0.2s;
  margin-right: 10px;
}
#btn8 {
  width: 150px;
  border-radius: 0;
  text-transform: none;
  height: 40px;
  transition: 0.2s;
  margin-right: 10px;
}
#btn9 {
  width: 150px;
  border-radius: 0;
  text-transform: none;
  height: 40px;
  transition: 0.2s;
}
#btnKadın {
  margin-right: 50px;
  width: 150px;
}
#btnErkek {
  margin-right: 500px;
  width: 150px;
}
#kampanya {
  width: 300px;
  margin-right: 500px;
}
</style>

<script>
import Carousel from "../components/CarouselHome.vue";
import Car2 from "../components/CarouselTeix.vue";
export default {
  name: "main",
  components: {
    Carousel,
    Car2,
  },
  data() {
    return {};
  },
};
</script>
