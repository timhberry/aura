<template>
  <v-content class="pa-0">

    <v-container fluid class="mt-3 mb-0">
      <v-layout wrap align-center justify-center row fill-height class="my-0">
        <v-flex xs12 md10 class="my-0">
            <p class="google-font mb-0" style="font-size:200%;color:#616161">Our noble organisers</p>
            <p class="google-font mt-0 mb-0" style="font-size:110%">These brave souls selflessly give up entire hours of their free time to organise GDG meetups, persitently nagging venue sponsors, ordering pizza, and bribing speakers with Swag. If you see them, just nod sagely, and know that they carry the weight of this medium-sized community group on their not inconsiderable shoulders.</p>
        </v-flex>
      </v-layout>
    </v-container>

    <v-container fluid >
      <v-layout wrap align-center justify-center row fill-height>
        <v-flex xs12 md10 class="">
          <coreTeam/>
        </v-flex>
      </v-layout>
    </v-container>

    <v-container fluid >
      <v-layout wrap align-center justify-center row fill-height>
        <v-flex xs12 md10 class="">
          <organizingTeam/>
        </v-flex>
      </v-layout>
    </v-container>

   


  </v-content>
  
</template>

<script>
import TeamDetails from '@/assets/data/chapterDetails.json'
import coreTeam from '@/components/team/coreTeam'
import organizingTeam from '@/components/team/organizingTeam'
  export default {
    components: {
      coreTeam,
      organizingTeam
    },
    data() {
      return {
        TeamDetails: TeamDetails,
      }
    },
  }
</script>
