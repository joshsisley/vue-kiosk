<template>
  <b-container class="steps-container bv-example-row">
    <b-row class="justify-content-md-center">
        <b-col cols="8" md="auto">
          <h1>Enter Your Information Below</h1>
          <p class="sub-header">Check in using your last name, first name and date of birth.</p>
          <div>
            <b-form @submit="onSubmit">
              <div class="input-container">
                <b-form-group id="exampleInputGroup2"
                      label-for="exampleInput2">
                  <b-form-input id="exampleInput2"
                        class="custom-input"
                        type="text"
                        size="lg"
                        required
                        placeholder="Last Name">
                  </b-form-input>
                </b-form-group>
                <b-form-group id="exampleInputGroup2"
                      label-for="exampleInput2">
                  <b-form-input id="exampleInput2"
                        class="custom-input"
                        type="text"
                        size="lg"
                        required
                        placeholder="First Name">
                  </b-form-input>
                </b-form-group> 
                <b-form-group id="exampleInputGroup2"
                      label-for="exampleInput2">
                  <b-form-input id="exampleInput2"
                        class="custom-input"
                        type="date"
                        size="lg"
                        required
                        placeholder="First Name">
                  </b-form-input>
                </b-form-group>
              </div>
              <b-button type="submit" class="btn-next">Next</b-button>
            </b-form>
          </div>
        </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {
  name: 'PatientInfo',
  methods: {
    onSubmit(evt) {
      evt.preventDefault();
      alert(JSON.stringify(this.form));
    }
  }
};
</script>

<style>
.input-container {
  padding: 30px 30px 17px 30px;
  background: white;
  border-radius: 6px;
  margin: 30px auto;
}
</style>
