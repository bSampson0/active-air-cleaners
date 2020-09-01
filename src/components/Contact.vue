<template>
  <v-container class="pb-15">
    <v-row class="intro pb-8 pt-10">
      <v-col cols="12" md="6">
        <h1>Where to find us!</h1>
        <p>
          Active Air Duct Cleaning is proud to service the Spokane, Washington
          area. Use the form to contact us today!
        </p>
        <h4>Spokane, Washington</h4>
        <p>
          620 W Persimmon Lane <br />
          Spokane, WA 99224 <br />
          Office: (541) 408-6001
        </p>
      </v-col>
      <v-col cols="12" md="6">
        <v-card class="custom-card mx-auto" max-width="500px">
          <v-card-title>
            <h2 class="pb-2">Contact Us</h2>
          </v-card-title>
          <v-card-subtitle>
            <h3 class="thin">
              Use the form below to claim your free quote.
            </h3>
          </v-card-subtitle>
          <v-card-text>
            <v-form class="post-form">
              <v-text-field
                v-model="name"
                label="Name"
                outlined
                required
              ></v-text-field>
              <v-text-field
                class="text-feild"
                v-model="email"
                label="Email"
                outlined
                required
              ></v-text-field>
              <v-text-field
                class="text-feild"
                v-model="phone"
                label="Phone"
                outlined
                required
              ></v-text-field>
              <v-text-field
                class="text-feild"
                v-model="sqft"
                label="Square footage of home."
                outlined
              >
              </v-text-field>
              <v-textarea
                v-model="message"
                outlined
                class="text-field"
                label="Message"
              ></v-textarea>
            </v-form>
          </v-card-text>
          <v-card-actions>
            <v-spacer></v-spacer>
            <v-btn color="#1E60E4" dark @click="submit">
              Submit
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data: () => ({
    name: null,
    email: null,
    phone: null,
    sqft: null,
    message: null
  })
};
</script>

<style lang="scss" scoped></style>
