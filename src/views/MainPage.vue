<template>
  <v-row>
    <v-col class="d-flex child-flex" cols="12" sm="12">
      <v-card>
        <v-img
          src="https://www.camper.com/cms/api/assets/tiers-banners-homes/2567a1e8-f454-4813-8004-31475bb67315/T93-MSS-noproduct-Desktop.avif"
          aspect-ratio="1"
          class="images"
        >
          <v-text class="sez"> Sezon Ortası İndirimi </v-text>
          <v-spacer></v-spacer>
          <v-text class="gifspan">%30'a Varan İndirim<br /> </v-text>
          <v-btn id="btnKadın" depressed> Kadın </v-btn>
          <v-btn id="btnErkek" depressed> Erkek </v-btn>
        </v-img>
      </v-card>
    </v-col>

    <v-col class="d-flex child-flex" cols="12" sm="12">
      <v-card>
        <v-img src="@/assets/camper_gif.gif" aspect-ratio="2" class="images">
          <v-text class="sez"> 11. Sayı Kıbrıs </v-text>
          <v-spacer></v-spacer>
          <v-text class="gifspan">The Walking Society<br /> </v-text>
          <v-spacer></v-spacer>
          <v-btn id="kampanya" depressed> Kampanyaya Göz Atın </v-btn>
        </v-img>
      </v-card>
    </v-col>

    <v-col class="d-flex child-flex" sm="12" cols="12">
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

    <v-col class="d-flex child-flex" cols="6">
      <v-card>
        <v-img
          :src="`https://www.camper.com/cms/api/assets/tiers-banners-homes/2429b0c7-0187-4d37-b5e4-ef9d3293b1ae/T93-Gender-Walden-Women-desktop.avif={}`"
          aspect-ratio="1"
          class="images"
        >
          <v-btn depressed elevation="2" floating class="butonlar" id="btn3"
            >Kadın</v-btn
          >
        </v-img>
      </v-card>
    </v-col>

    <v-col class="d-flex child-flex" cols="6">
      <v-img
        :src="`https://www.camper.com/cms/api/assets/tiers-banners-homes/7cf1e10a-0c2f-4505-9835-c52f97182916/T93-Gender-Walden-Men-desktop.avif={}`"
        aspect-ratio="1"
        class="images"
      >
        <v-btn depressed elevation="2" floating class="butonlar" id="btn4"
          >Erkek</v-btn
        >
      </v-img>
    </v-col>

    <v-col class="d-flex child-flex" cols="12">
      <v-img
        :src="`https://www.camper.com/cms/api/assets/tiers-banners-homes/c565ea73-9386-4b44-bd51-8389176cde27/T93_Store-locator-Dist-desktop.avif={}`"
        aspect-ratio="2"
        class="images"
      >
        <v-btn depressed elevation="2" floating class="butonlar" id="btn5"
          >En Yakın Mağazayı Bul</v-btn
        >
      </v-img>
    </v-col>
  </v-row>
</template>

<style scoped >
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
  margin-right: 550px;
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
  margin-right: 720px;
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
export default {
  name: "main",
  data() {
    return {};
  },
};
</script>
