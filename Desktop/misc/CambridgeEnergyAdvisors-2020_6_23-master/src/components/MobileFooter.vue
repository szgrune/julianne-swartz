<template>
    <div class="text-center content-body">
        <div class="d-flex flex-column"
        @click="sheet = !sheet">
            <span class="mt-4 mb-2"> 
                <strong> 
                <v-icon>
                    mdi-chevron-up
                </v-icon>
                </strong>
            </span>
            <span>
                <strong>Contact</strong>
            </span>
        </div>
    <v-bottom-sheet v-model="sheet">
      <v-sheet class="text-center" height="">
        <v-icon
          class="mt-6"
          text
          color="red"
          @click="sheet = !sheet"
        >mdi-chevron-down</v-icon>
        <v-container class="px-8 d-flex flex-column text-center content-body">
            <v-row class="text-left">
                <span class="text-white">Cambridge Energy Advisors</span>
                 <p class="grey-text text-lighten-4">
                    Principal: Eric Grunebaum <br>
                    <a href="https://www.linkedin.com/in/ericgrunebaum/"><v-icon>mdi-linkedin</v-icon></a>
                    <a href="mailto:eric@cambridgeenergyadvisors.com"><v-icon>mdi-email</v-icon></a>
                    <a href="tel:617-304-5824"><v-icon>mdi-phone</v-icon></a><br>                                        
                </p>
            </v-row>
            <v-divider></v-divider>
            <v-row class="py-4 text-left">
                 <p class="grey-text text-lighten-4">
                    Cambridge Innovation Center<br>
                    1 Broadway, 14th Floor<br>
                    Cambridge, MA 02142
                </p>
            </v-row>
            <v-divider></v-divider>
            <v-row class="py-4 text-left">
                <p class="grey-text text-lighten-4">
                    Securities offered through:<br> 
                    Pickwick Capital Partners, LLC Member FINRA/SIPC<br>
                    445 Hamilton Ave, Suite 1102,<br>
                    White Plains, NY, 10601<br>
                    Office: (914) 358-3269<br>
                    Direct: (617) 304-5824<br>
                    <a id="broker" target="_blank" href="https://brokercheck.finra.org/individual/summary/6593435">Broker Check</a>
                </p>
            </v-row>
    </v-container>
      </v-sheet>
    </v-bottom-sheet>
    </div>
</template>
<script>
export default {
    data: () => ({
        sheet: false
    })
    
}
</script>
<style scoped>
    .content-body {
        font-size: 1.3rem;
    }
    a{
        text-decoration: none;
    }
    #broker{
        text-decoration: underline;
        color: #000000de;
    }
</style>