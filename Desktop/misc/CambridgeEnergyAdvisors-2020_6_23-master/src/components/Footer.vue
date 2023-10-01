<template>
    <v-footer
      padless
      class="font-weight-light primary justify-center"
    >
    <!-- Social media? -->
    <v-container class="d-none d-sm-flex text-center main-text">
            <v-col class="text-left">
                <span class="text-white">Cambridge Energy Advisors</span><br>
                <span class="text-white">Pickwick Capital Partners, LLC</span>
                 <p class="grey-text text-lighten-4">
                    Managing Director: Eric Grunebaum  
                </p>
                <a href="tel:617-304-5824"><v-icon>mdi-phone</v-icon></a>
                <a href="mailto:eric@cambridgeenergyadvisors.com"><v-icon>mdi-email</v-icon></a>
                <a target="_blank" href="https://www.linkedin.com/in/ericgrunebaum/"><v-icon>mdi-linkedin</v-icon></a>
            </v-col>
            <v-col class="text-left">
                 <p class="grey-text text-lighten-4">
                    
                </p>
            </v-col>
            <v-col class="text-left">
                <p class="grey-text text-lighten-4">
                    Securities offered through:<br> 
                    Eric Grunebaum | Managing Director<br>
                    Pickwick Capital Partners, LLC<br>
                    445 Hamilton Ave, Suite 1102,<br>
                    White Plains, NY, 10601<br>
                    Office: (914) 358-3269<br>
                    Direct: (617) 304-5824<br>

                    <a href="mailto:grunebaume@pickwickcapital.com"><v-icon>mdi-email</v-icon></a>
                </p>
                <a style="color: black;" target="_blank" href="https://pickwickcapitalpartners.com">www.pickwickcapitalpartners.com</a><br>
                <a style="color: black;" target="_blank" href="https://brokercheck.finra.org/individual/summary/6593435">Broker Check</a>
            </v-col>
    </v-container>
    <mobile-footer  class="hidden-sm-and-up"></mobile-footer>
    <v-container class="d-flex text-center flex-column">
        <v-col> &copy; {{ new Date().getFullYear() }} — <strong>Cambridge Energy Advisors</strong></v-col>
        <p class="fine-print-m grey-text text-lighten-4 hidden-sm-and-up"><em>Cambridge Energy Advisors is not an investment advisor and does not provide investment advice. All securities-related activities are conducted by Eric Grunebaum, a registered representative of Pickwick Capital Partners LLC, Member FINRA/SIPC.</em></p>
        <p class="fine-print grey-text text-lighten-4 hidden-xs-only"><em>Cambridge Energy Advisors is not an investment advisor and does not provide investment advice. All securities-related activities are conducted by Eric Grunebaum, a registered representative of Pickwick Capital Partners LLC, Member FINRA/SIPC.</em></p>
    </v-container>
    
    </v-footer>
</template>
<script>
import MobileFooter from './MobileFooter'
export default {
    components:{
        'mobile-footer': MobileFooter
    }
}
</script>
<style scoped>
    .main-text {
        font-size: 1.15rem
    }

    .fine-print-m {
        font-size: .75rem;
    }
    .fine-print {
        font-size: .95rem;
    }
</style>