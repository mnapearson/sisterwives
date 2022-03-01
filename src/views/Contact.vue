<template>
  <div>
    <!-- <h1>
      <a class="link" href="mailto:info@sisterwives.studio"
        >info@sisterwives.studio</a
      >
    </h1> -->
    <p>get in touch</p>
    <div class="contact-form">
      <form
        ref="contact"
        class="contact-form"
        @submit.prevent="sendEmail"
        v-if="!successMessage"
      >
        <input class="field" type="text" name="user_name" placeholder="name" />

        <input
          class="field"
          type="email"
          name="user_email"
          placeholder="email"
        />

        <textarea class="field" name="message" placeholder="message"></textarea>
        <input class="field submit" type="submit" value="Send" />
      </form>
      <p v-if="successMessage">
        Thank you for your message. <br />We will get back to you soon.
      </p>
    </div>
  </div>
</template>

<script>
import emailjs from "emailjs-com";

export default {
  name: "Contact",
  data() {
    return {
      name: "",
      email: "",
      message: "",
      successMessage: false,
    };
  },
  methods: {
    sendEmail(e) {
      try {
        emailjs.sendForm(
          "service_9kxr7d6",
          "template_trxnvmr",
          e.target,
          "user_o6tM95YAVRykwYE7z90AI",
          {
            name: this.name,
            email: this.email,
            message: this.message,
          }
        );
      } catch (error) {
        console.log({ error });
      }
      // Reset form field
      this.name = "";
      this.email = "";
      this.message = "";
      this.successMessage = true;
    },
  },
};
</script>

<style scoped>
h1 {
  -webkit-animation: fade-in 1.75s cubic-bezier(0.39, 0.575, 0.565, 1) both;
  animation: fade-in 1.75s cubic-bezier(0.39, 0.575, 0.565, 1) both;
}

.contact-form {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-left: 2rem;
}

.field {
  width: 250px;
  margin: 1rem;
  padding: 0.5rem;
  border-radius: 5px;
  background-color: #e9e9e9;
  font-family: "Metana";
  cursor: crosshair;
}

.submit {
  cursor: pointer;
}

textarea {
  height: 150px;
}

p {
  margin-top: 3rem;
  font-size: 18px;
}
</style>
