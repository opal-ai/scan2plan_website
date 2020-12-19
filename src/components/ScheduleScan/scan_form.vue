<!-- @format -->

<template>
  <div class="scan_form" id="grad">
    <b-container>
      <b-row>
        <h1>ORDER SCANS</h1>
      </b-row>
      <b-row>
        <b-col>
          <h3>
            PERSONAL DETAILS
          </h3>

          <b-form @submit="onSubmit" @reset="onReset" v-if="show">
            <b-form-group
              id="input-group-1"
              label="Your Name:"
              label-for="input-1"
            >
              <b-form-input
                id="input-1"
                v-model="form.name"
                required
                placeholder="Enter name"
              ></b-form-input>
            </b-form-group>
            <b-form-group
              id="input-group-2"
              label="Email address:"
              label-for="input-2"
            >
              <b-form-input
                id="input-2"
                v-model="form.email"
                type="email"
                required
                placeholder="Enter email"
              ></b-form-input>
            </b-form-group>

            <b-form-group
              id="input-group-3"
              label="Phone number:"
              label-for="input-3"
            >
              <b-form-input
                id="input-3"
                v-model="form.Phone"
                type="Phone"
                required
                placeholder="Enter phone number"
              ></b-form-input>
            </b-form-group>

            <!-- <b-button type="submit" variant="primary">Submit</b-button> -->
            <!-- <b-button type="reset" variant="danger">Reset</b-button> -->
          </b-form>
        </b-col>
        <b-col>
          <h3>
            LOCATION DETAILS
          </h3>
          <form>
            <b-container>
              <b-row>
                <div class="form-group">
                  <!-- Street 1 -->
                  <label for="street1_id" class="control-label"
                    >Street Address 1</label
                  >
                  <input
                    type="text"
                    class="form-control"
                    id="street1_id"
                    name="street1"
                    placeholder="Street address, P.O. box, company name, c/o"
                  />
                </div>
              </b-row>
              <b-row>
                <div class="form-group">
                  <!-- Street 2 -->
                  <label for="street2_id" class="control-label"
                    >Street Address 2</label
                  >
                  <input
                    type="text"
                    class="form-control"
                    id="street2_id"
                    name="street2"
                    placeholder="Apartment, suite, unit, building, floor, etc."
                  />
                </div>
              </b-row>
              <b-row>
                <b-col>
                  <div class="form-group">
                    <!-- City-->
                    <label for="city_id" class="control-label">City</label>
                    <input
                      type="text"
                      class="form-control"
                      id="city_id"
                      name="city"
                      placeholder="Smallville"
                    />
                  </div>
                </b-col>
                <b-col>
                  <div class="form-group">
                    <!-- State Button -->
                    <label for="state_id" class="control-label">State</label>
                    <select class="form-control" id="state_id">
                      <option value="AL">Alabama</option>
                      <option value="AK">Alaska</option>
                      <option value="AZ">Arizona</option>
                      <option value="AR">Arkansas</option>
                      <option value="CA">California</option>
                      <option value="CO">Colorado</option>
                      <option value="CT">Connecticut</option>
                      <option value="DE">Delaware</option>
                      <option value="DC">District Of Columbia</option>
                      <option value="FL">Florida</option>
                      <option value="GA">Georgia</option>
                      <option value="HI">Hawaii</option>
                      <option value="ID">Idaho</option>
                      <option value="IL">Illinois</option>
                      <option value="IN">Indiana</option>
                      <option value="IA">Iowa</option>
                      <option value="KS">Kansas</option>
                      <option value="KY">Kentucky</option>
                      <option value="LA">Louisiana</option>
                      <option value="ME">Maine</option>
                      <option value="MD">Maryland</option>
                      <option value="MA">Massachusetts</option>
                      <option value="MI">Michigan</option>
                      <option value="MN">Minnesota</option>
                      <option value="MS">Mississippi</option>
                      <option value="MO">Missouri</option>
                      <option value="MT">Montana</option>
                      <option value="NE">Nebraska</option>
                      <option value="NV">Nevada</option>
                      <option value="NH">New Hampshire</option>
                      <option value="NJ">New Jersey</option>
                      <option value="NM">New Mexico</option>
                      <option value="NY">New York</option>
                      <option value="NC">North Carolina</option>
                      <option value="ND">North Dakota</option>
                      <option value="OH">Ohio</option>
                      <option value="OK">Oklahoma</option>
                      <option value="OR">Oregon</option>
                      <option value="PA">Pennsylvania</option>
                      <option value="RI">Rhode Island</option>
                      <option value="SC">South Carolina</option>
                      <option value="SD">South Dakota</option>
                      <option value="TN">Tennessee</option>
                      <option value="TX">Texas</option>
                      <option value="UT">Utah</option>
                      <option value="VT">Vermont</option>
                      <option value="VA">Virginia</option>
                      <option value="WA">Washington</option>
                      <option value="WV">West Virginia</option>
                      <option value="WI">Wisconsin</option>
                      <option value="WY">Wyoming</option>
                    </select>
                  </div>
                </b-col>
              </b-row>
              <b-row>
                <b-col>
                  <div class="form-group">
                    <!-- Country Button -->
                    <label for="country_id" class="control-label"
                      >Country</label
                    >
                    <select class="form-control" id="country_id">
                      <option value="AL">United States</option>
                    </select>
                  </div>
                </b-col>
                <b-col>
                  <div class="form-group">
                    <!-- Zip Code-->
                    <label for="zip_id" class="control-label">Zip Code</label>
                    <input
                      type="text"
                      class="form-control"
                      id="zip_id"
                      name="zip"
                      placeholder="#####"
                    />
                  </div>
                </b-col>
              </b-row>
              <b-row>
                <div class="form-group">
                  <!-- Submit Button -->
                  <button type="submit" class="btn btn-primary">
                    Make an order
                  </button>
                </div>
              </b-row>
            </b-container>
          </form>
        </b-col>

        <b-col>
          <h3>
            SCHEDULE
          </h3>
          <b-container>
            <b-row>
              <datepicker :inline="true"></datepicker>
            </b-row>
            <b-row>
              <b-form-timepicker
                class="time_style"
                v-model="value"
                locale="en"
              ></b-form-timepicker>
            </b-row>
          </b-container>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import Datepicker from 'vuejs-datepicker';
export default {
  components: {
    Datepicker,
  },
  name: 'ScanForm',
  props: {},
  data() {
    return {
      form: {
        email: '',
        name: '',
        food: null,
        checked: [],
      },
      foods: [
        { text: 'Select One', value: null },
        'Carrots',
        'Beans',
        'Tomatoes',
        'Corn',
      ],
      show: true,
    };
  },
  methods: {
    onSubmit(evt) {
      evt.preventDefault();
      alert(JSON.stringify(this.form));
    },
    onReset(evt) {
      evt.preventDefault();
      // Reset our form values
      this.form.email = '';
      this.form.name = '';
      this.form.food = null;
      this.form.checked = [];
      // Trick to reset/clear native browser form validation state
      this.show = false;
      this.$nextTick(() => {
        this.show = true;
      });
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
#grad {
  background-image: linear-gradient(white, rgb(209, 220, 240));
}
.time_style {
  margin-top: 2vh;
}
</style>
