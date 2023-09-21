<template>
  <div class="contact_container">
    <div class="contact_text_container">
      <p class="contact_head_text">Let's chat.</p>
      <p class="contact_head_text">Tell me about your</p>
      <p class="contact_head_text">project.</p>
      <p class="contact_sub_text">Let's create something great together ✌️</p>
    </div>
    <div class="contact_table_container">
      <table class="form_fields_container">
        <tr>
          <td><InputForm :form_title="'name'" /></td>
        </tr>
        <tr>
          <td><InputForm :form_title="'email'" /></td>
        </tr>
        <tr>
          <td>
            <div>
              <textarea
                class="message_form"
                name="messege_text"
                id="mtext"
                cols="30"
                rows="10"
                placeholder="Enter your messege"
              ></textarea>
            </div>
          </td>
        </tr>
        <tr>
            <td>
                <button class="send_button" @click="finishMessage">
                    Send
                </button>
            </td>
        </tr>
      </table>
    </div>
  </div>
</template>

<script>
import InputForm from "./InputForm.vue";
export default {
  name: "ContactSection",
  components: {
    InputForm,
  },

  methods:{
    finishMessage()
    {
      this.$router.push("/contact-final");
    }
  }
};
</script>

<style>

</style>
