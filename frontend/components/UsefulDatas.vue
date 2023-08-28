<template>
  <div class="datasContainer">
    <div class="projects">
      <div class="leftColumn">
        <div class="linksTitle">
          <div class="usefulLinks">
            <span>Les liens utiles</span>
            <div class="surlignage"></div>
          </div>
        </div>
        <div class="capsuleContainerL">
          <div class="capsule greenit">
            <img :src="logoGreenIT" alt="Green IT" />
          </div>
        </div>
        <div class="capsuleContainerL">
          <div class="capsule fairphone">
            <img :src="logoFairphone" alt="Fairphone" />
          </div>
        </div>
      </div>
      <div class="rightColumn">
        <div class="capsuleContainerR">
          <div class="capsule agit">
            <img :src="logoAgit" alt="AGIT" />
          </div>
        </div>
        <div class="capsuleContainerR">
          <div class="capsule shift">
            <img :src="logoShift" alt="The Shift Project" />
          </div>
        </div>
        <div class="capsuleContainerR">
          <div class="capsule backmarket">
            <img :src="logoBackmarket" alt="Back Market" />
          </div>
        </div>
      </div>
    </div>
    <div class="numbersContainer">
      <span class="sectionTitle">L'impact du numérique</span>
      <h1>Découvrez quelques chiffres clés</h1>
      <div class="numbers">
        <div class="w50p">
          <div class="numericData">
            <div class="backgroundData"></div>
            <span>11</span>
          </div>
          <span>Equipements par français en moyenne</span>
        </div>
        <div class="w50p">
          <div class="numericData">
            <div class="backgroundData"></div>
            <span>4%</span>
          </div>
          <span>De l'empreinte humaine mondiale en 2020</span>
        </div>
        <div class="w50p">
          <div class="numericData w75p">
            <div class="backgroundData"></div>
            <span>4 à 6 ans</span>
          </div>
          <span>Durée de vie d'un terminal en 2022 contre 10 à 15 ans en 1995</span>
        </div>
        <div class="w50p">
          <div class="numericData">
            <div class="backgroundData"></div>
            <span>6</span>
          </div>
          <span>Limites planétaires sur 9 déjà dépassées</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  import logoAgit from "@/assets/images/agit.png";
  import logoBackmarket from "@/assets/images/backmarket.png";
  import logoFairphone from "@/assets/images/fairphone.png";
  import logoGreenIT from "@/assets/images/greenit.png";
  import logoShift from "@/assets/images/shift.png";
  export default {
    name: 'UsefulDatas',
    setup() {
      return {
        logoAgit,
        logoBackmarket,
        logoFairphone,
        logoGreenIT,
        logoShift
      };
    }
  }
</script>

<style scoped>
  @import "@/assets/css/datas.css"
</style>