<template>
  <div class="form_container">
    <!-- <div class="form_title_container">
            <p class="form_title_text">{{ form_title }}</p>
        </div> -->
    <div class="form_field_container">
      <form action="">
        <input
          class="input_field"
          type="text"
          id="fname"
          name="fname"
          :placeholder="'Enter your ' + form_title + ''"
        /><br />
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: "InputForm",
  props: {
    form_title: String,
  },
};
</script>

<style>
.form_container {
  display: flex;
  flex-direction: column;
}

.form_title_container {
  display: flex;
}

.form_title_text {
  margin: 0;
  padding: 5px 0;
}

/* .form_fiedld_container {
} */

.input_field {
  font-family: inherit;
  border: 3px solid #9ba4b5;
  outline: 0;
  font-size: 1.3rem;
  color: #263228;
  background: transparent;
  transition: border-color 0.2s;
  border-radius: 7px;
}

.input_field:focus{
    border-color: #6c63ff;
}

.input_field::placeholder {
  font-size: 1.3rem;
}
</style>