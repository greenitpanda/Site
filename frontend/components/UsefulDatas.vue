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
            <a href="https://www.greenit.fr/">
              <img :src="logoGreenIT" alt="Green IT" />
            </a>
          </div>
        </div>
        <div class="capsuleContainerL">
          <div class="capsule fairphone">
            <a href="https://www.fairphone.com/fr/">
              <img :src="logoFairphone" alt="Fairphone" />
            </a>
          </div>
        </div>
      </div>
      <div class="rightColumn">
        <div class="capsuleContainerR">
          <div class="capsule agit">
            <a href="https://alliancegreenit.org/">
              <img :src="logoAgit" alt="AGIT" />
            </a>
          </div>
        </div>
        <div class="capsuleContainerR">
          <div class="capsule shift">
            <a href="https://theshiftproject.org/">
              <img :src="logoShift" alt="The Shift Project" />
            </a>
          </div>
        </div>
        <div class="capsuleContainerR">
          <div class="capsule backmarket">
            <a href="https://www.backmarket.fr/fr-fr">
              <img :src="logoBackmarket" alt="Back Market" />
            </a>
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
            <img class="eleven" :src="eleven" />
          </div>
          <span>Equipements par français en moyenne</span>
        </div>
        <div class="w50p">
          <div class="numericData">
            <div class="backgroundData"></div>
            <img class="fourpercent" :src="fourpercent" />
          </div>
          <span>De l'empreinte humaine mondiale en 2020</span>
        </div>
        <div class="w50p">
          <div class="numericData w100p">
            <div class="backgroundData"></div>
            <img class="dureeVie" :src="dureeVie" />
          </div>
          <span>Durée de vie d'un terminal en 2022 contre 10 à 15 ans en 1995</span>
        </div>
        <div class="w50p">
          <div class="numericData">
            <div class="backgroundData"></div>
            <img class="numeroSix" :src="numeroSix" />
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
  import eleven from "@/assets/images/11.png";
  import fourpercent from "@/assets/images/4percent.png";
  import dureeVie from "@/assets/images/duree_vie.png";
  import numeroSix from "@/assets/images/numero6.svg";
  export default {
    name: 'UsefulDatas',
    setup() {
      return {
        logoAgit,
        logoBackmarket,
        logoFairphone,
        logoGreenIT,
        logoShift,
        eleven,
        fourpercent,
        dureeVie,
        numeroSix
      };
    }
  }
</script>

<style scoped>
  @import "@/assets/css/datas.css"
</style>