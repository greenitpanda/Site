<template>
  <div class="containerContact">
    <div class="infoContact">
      <h2>N'hésitez pas à nous contacter pour échanger sur vos projets :</h2>
      <span class="companyName">Green IT Panda</span><br/>
      <span>
        1400 route du bourg<br/>
        71500 BRUAILLES<br/>
        +33 6 86 01 62 59<br/>
        contact[at]greenitpanda.fr
      </span>
    </div>
    <div class="containerForm">
      <h2>Formulaire de contact :</h2>
      
      <form id="myForm">
        <label>Nom</label>
        <input 
          v-model="name"
          type="text" 
          name="name"
          class="inputForm"
        >
        <label>Prénom</label>
        <input 
          v-model="surname"
          type="text" 
          name="surname"
          class="inputForm"
        >
        <label>E-mail</label>
        <input 
          v-model="email"
          type="email" 
          name="email"
          class="inputForm"
          >
        <label>Téléphone</label>
        <input 
          v-model="phone"
          type="text" 
          name="phone"
          class="inputForm"
          >
        <label>Votre message</label>
        <textarea 
          v-model="message"
          name="message"
          class="message"
          cols="30" rows="10">
        </textarea>
        <div id="error" class="sendingResult sendingError">Une erreur est survenur durant l'envoi du mail.</div>
        <div id="sent" class="sendingResult sendingDone">Votre demande a bien été envoyée ! Notre équipe revient vers vous dans les meilleurs délais.</div>
        <button type="button" class="buttonSend" @click="sendEmail">Envoyer</button>
      </form>
    </div>
  </div>
</template>

<script>
  import {sendForm} from 'emailjs-com';
  export default {
    name: 'ContentContact',
    setup() {
      return {
        name: '',
        surname: '',
        email: '',
        phone: '',
        message: ''
      };
    },
    methods: {
      sendEmail(e) {
        try {
          sendForm('service_ecwpyhd', 'template_whez7sf', '#myForm', 'CmWnd60ndh9aIndoR')
            .then(function() {
              document.getElementById("sent").classList.toggle("sendingFinished");
            }).catch(function(){
              document.getElementById("error").classList.toggle("sendingFinished");
            });
        } catch(error) {
          this.erreurSend = true;
        }
      },
    }
  }
</script>

<style scoped>
  @import "@/assets/css/contact.css"
</style>
