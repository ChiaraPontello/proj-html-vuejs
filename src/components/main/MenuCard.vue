<template>
    <div class="container">
    <div class="d-flex justify-content-between ">

      <!--1°menu-->
        <div class="boxSide">
          <div>
            <h1>HORS D’OEUVRES</h1>
            <div v-for="(plate, i) in firstList" :key="i">
              <div>
                <h4 class="py-3">{{ plate.name }}</h4>
                <span>{{ plate.price }}</span>
              </div>
              <p>{{ plate.text }}</p>
            </div>
            
          </div>
        </div>
      
      <!--2°menu-->
      <div class="boxCenter ">
        <div class=" text-light">
          <h1>MAIN COURSE</h1>
            <div v-for="(plate, i) in secondList" :key="i">
              <div >
                <h4 class="py-3">{{ plate.name }}</h4>
                <span>{{ plate.price }}</span>
              </div>
              <p>{{ plate.text }}</p>
            </div>
          
        </div>
      </div>

      <!--3°menu-->
      <div class="boxSide ">
        <div>
            <h1>DESSERTS</h1>
            <div v-for="(plate, i) in thirdList" :key="i">
              <div >
                <h4 class="py-3">{{ plate.name }}</h4>
                <span>{{ plate.price }}</span>
              </div>
              <p>{{ plate.text }}</p>
            </div>
            
          </div>
      </div>
    </div>
    </div>
</template>

<script>
    export default {
        name: 'MenuCard',
        data() {
        return {
           firstList: [
        {
          name: "AHI SALMON NIGIRI",
          price: "$48",
          text: "Mollis ornare sit sapien, sodales. Cursus duis proin semper quisque.",
        },
        {
          name: "UMI MASU SALAD",
          price: "$21",
          text: "Mollis ornare sit sapien, sodales. Cursus duis proin semper quisque.",
        },
        {
          name: "TEMAKI WITH CRAB",
          price: "$32",
          text: "Mollis ornare sit sapien, sodales. Cursus duis proin semper quisque.",
        },
        {
          name: "CALIFORNIA ROLLS",
          price: "$22",
          text: "Mollis ornare sit sapien, sodales. Cursus duis proin semper quisque.",
        },
      ],

      secondList: [
        {
          name: "BRAISED ABALONE",
          price: "$52",
          text: "Mollis ornare sit sapien, sodales. Cursus duis proin semper quisque.",
        },
        {
          name: "TWICE COOKED PORK",
          price: "$21",
          text: "Mollis ornare sit sapien, sodales. Cursus duis proin semper quisque.",
        },
        {
          name: "KUNG PAO CHICKEN",
          price: "$32",
          text: "Mollis ornare sit sapien, sodales. Cursus duis proin semper quisque.",
        },
        {
          name: "CHAR SIU & SUSHI",
          price: "$48",
          text: "Mollis ornare sit sapien, sodales. Cursus duis proin semper quisque.",
        },
      ],

      thirdList: [
        {
          name: "CHOCOLATE BALL CAKE",
          price: "$13",
          text: "Mollis ornare sit sapien, sodales. Cursus duis proin semper quisque.",
        },
        {
          name: "LIME PIE WITH CRUST",
          price: "$14",
          text: "Mollis ornare sit sapien, sodales. Cursus duis proin semper quisque.",
        },
        {
          name: "RASPBERRY PEAR CAKE",
          price: "$18",
          text: "Mollis ornare sit sapien, sodales. Cursus duis proin semper quisque.",
        },
        {
          name: "CAFÉ AU LAIT",
          price: "$6",
          text: "Mollis ornare sit sapien, sodales. Cursus duis proin semper quisque.",
        },
      ],
    }
    }
}
</script>

<style lang="scss" scoped>

  .boxSide {
  background-color: rgb(232, 232, 232);
  width: 45%;
  height: 105vh;
  padding: 40px;
  margin-top: 30px;
}
.boxCenter {
  background-color: black;
  width: 45%;
  height: 105vh;
  padding: 40px;
}
span{
  float: right;
}

</style>