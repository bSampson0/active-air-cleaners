<template>
  <div class="services">
    <v-container class="pb-15 pt-10">
      <v-row class="intro pb-5 pt-10">
        <v-col>
          <h1>What we offer.</h1>
          <p>
            Active Air Duct Cleaning recommends that every customer that has
            ducts in their home or business have them cleaned regularly to
            reduce the spread of allergens, bacteria, pollutants, and dust which
            can lead to respiratory problems and sneezing.
          </p>
        </v-col>
      </v-row>

      <v-row>
        <v-col cols="12" md="6" class="d-flex" align="center">
          <v-img
            class="left-img"
            aspect-ratio="1"
            src="https://images.unsplash.com/photo-1590620284812-3216c0ea0a75?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2702&q=80"
          ></v-img>
        </v-col>
        <v-col cols="12" md="6">
          <v-row>
            <v-col cols="12">
              <h2 class="pb-4">
                <span style="font-weight: 300">Active Air</span> Cleaning
                Services
              </h2>
              <p>
                Cleaning your air ducts eliminates contaminants and dust that
                can circulate throughout your home every time your HVAC system
                is used, causing issues for people who are sensitive to airborne
                particles. Regular cleaning of the ducts in your home or office
                can also improve the performance of your heating and air
                conditioning system and increase its service life.
              </p>
            </v-col>
            <v-col
              cols="12"
              md="6"
              v-for="service in services"
              v-bind:key="service.key"
            >
              <h3 class="pb-2">{{ service.name }}</h3>
              <p>{{ service.description }}</p>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  data: () => ({
    services: [
      {
        name: "Air Duct Cleaning",
        description:
          "Experienced technicians will rid your home of allergens & unsightly dust using our industry leading duct cleaning equipment.",
        imgUrl:
          "https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRC7NuZIrFs7z6UYI-LaAfaLYHJWnnR3bHoHA&usqp=CAU"
      },
      {
        name: "Dryer Duct Cleaning",
        description:
          "Dryer lint build-up can become a real fire hazard. Our experienced technicians will return your dryer ducts to like-new condition.",
        imgUrl:
          "https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRC7NuZIrFs7z6UYI-LaAfaLYHJWnnR3bHoHA&usqp=CAU"
      },
      {
        name: "Ozone Treatment",
        description:
          "Expert technicians completely remove nasty odors at the molecular level, using the industry’s most powerful ozone generator. In addition to odor elimination, ozone has the potential to be an incredibly effective disinfectant. Our team can treat any size space to ensure your family or customers are safe.",
        imgUrl:
          "https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRC7NuZIrFs7z6UYI-LaAfaLYHJWnnR3bHoHA&usqp=CAU"
      },
      {
        name: "Air Duct Sanitizing",
        description:
          "Our team will use our innovative duct sanitizing system to apply a microbiostatic solution directly to your duct walls, killing up to 99.9% of viruses, bacteria, and mold.",
        imgUrl:
          "https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRC7NuZIrFs7z6UYI-LaAfaLYHJWnnR3bHoHA&usqp=CAU"
      }
    ]
  })
};
</script>

<style lang="scss" scoped>
.services {
  background: #eee;
}
</style>
