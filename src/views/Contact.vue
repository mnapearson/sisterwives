<template>
  <div>
    <!-- <h1>
      <a class="link" href="mailto:info@sisterwives.studio"
        >info@sisterwives.studio</a
      >
    </h1> -->
    <h3>get in touch</h3>
    <form
      ref="contact"
      class="contact-form"
      @submit.prevent="sendEmail"
      v-if="!successMessage"
    >
      <input
        class="field"
        type="text"
        name="user_name"
        placeholder="name"
        required
      />

      <input
        class="field"
        type="email"
        name="user_email"
        placeholder="email"
        required
      />

      <textarea
        class="field"
        name="message"
        placeholder="message"
        required
      ></textarea>
      <input class="field submit" type="submit" value="Send" />
    </form>
    <p v-if="successMessage">
      Thank you for your message. <br />We will get back to you soon.
    </p>
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
.contact-form {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.field {
  width: 350px;
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

h3 {
  text-align: center;
}
</style>
