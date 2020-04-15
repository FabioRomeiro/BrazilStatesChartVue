<template>
    <svg width="798" height="756" viewBox="0 0 798 756" fill="none" xmlns="http://www.w3.org/2000/svg">
        <AC 
            @click.native="click('AC')"
            @mouseover.native="mouseover('AC')"
        />
        <AL 
            @click.native="click('AL')"
            @mouseover.native="mouseover('AL')"
        />
        <AM 
            @click.native="click('AM')"
            @mouseover.native="mouseover('AM')"
        />
        <AP 
            @click.native="click('AP')"
            @mouseover.native="mouseover('AP')"
        />
        <BA 
            @click.native="click('BA')"
            @mouseover.native="mouseover('BA')"
        />
        <CE 
            @click.native="click('CE')"
            @mouseover.native="mouseover('CE')"
        />
        <DF 
            @click.native="click('DF')"
            @mouseover.native="mouseover('DF')"
        />
        <ES 
            @click.native="click('ES')"
            @mouseover.native="mouseover('ES')"
        />
        <GO 
            @click.native="click('GO')"
            @mouseover.native="mouseover('GO')"
        />
        <MA 
            @click.native="click('MA')"
            @mouseover.native="mouseover('MA')"
        />
        <MG 
            @click.native="click('MG')"
            @mouseover.native="mouseover('MG')"
        />
        <MS 
            @click.native="click('MS')"
            @mouseover.native="mouseover('MS')"
        />
        <MT 
            @click.native="click('MT')"
            @mouseover.native="mouseover('MT')"
        />
        <PA 
            @click.native="click('PA')"
            @mouseover.native="mouseover('PA')"
        />
        <PB 
            @click.native="click('PB')"
            @mouseover.native="mouseover('PB')"
        />
        <PE 
            @click.native="click('PE')"
            @mouseover.native="mouseover('PE')"
        />
        <PI 
            @click.native="click('PI')"
            @mouseover.native="mouseover('PI')"
        />
        <PR 
            @click.native="click('PR')"
            @mouseover.native="mouseover('PR')"
        />
        <RJ 
            @click.native="click('RJ')"
            @mouseover.native="mouseover('RJ')"
        />
        <RN 
            @click.native="click('RN')"
            @mouseover.native="mouseover('RN')"
        />
        <RO 
            @click.native="click('RO')"
            @mouseover.native="mouseover('RO')"
        />
        <RR 
            @click.native="click('RR')"
            @mouseover.native="mouseover('RR')"
        />
        <RS 
            @click.native="click('RS')"
            @mouseover.native="mouseover('RS')"
        />
        <SC 
            @click.native="click('SC')"
            @mouseover.native="mouseover('SC')"
        />
        <SE 
            @click.native="click('SE')"
            @mouseover.native="mouseover('SE')"
        />
        <SP 
            @click.native="click('SP')"
            @mouseover.native="mouseover('SP')"
        />
        <TO 
            @click.native="click('TO')"
            @mouseover.native="mouseover('TO')"
        />
    </svg>
</template>

<script>
import AC from './States/AC.vue'
import AL from './States/AL.vue'
import AM from './States/AM.vue'
import AP from './States/AP.vue'
import BA from './States/BA.vue'
import CE from './States/CE.vue'
import DF from './States/DF.vue'
import ES from './States/ES.vue'
import GO from './States/GO.vue'
import MA from './States/MA.vue'
import MG from './States/MG.vue'
import MS from './States/MS.vue'
import MT from './States/MT.vue'
import PA from './States/PA.vue'
import PB from './States/PB.vue'
import PE from './States/PE.vue'
import PI from './States/PI.vue'
import PR from './States/PR.vue'
import RJ from './States/RJ.vue'
import RN from './States/RN.vue'
import RO from './States/RO.vue'
import RR from './States/RR.vue'
import RS from './States/RS.vue'
import SC from './States/SC.vue'
import SE from './States/SE.vue'
import SP from './States/SP.vue'
import TO from './States/TO.vue'

export default {
    name: 'Brazil',
    components: {
        AC,
        AL,
        AM,
        AP,
        BA,
        CE,
        DF,
        ES,
        GO,
        MA,
        MG,
        MS,
        MT,
        PA,
        PB,
        PE,
        PI,
        PR,
        RJ,
        RN,
        RO,
        RR,
        RS,
        SC,
        SE,
        SP,
        TO,
    },
    data() {
        return {
            selectedState: undefined
        };
    },
    methods: {
        click(state) {
            
            console.log('Clicou no', state)

            if (state === this.selectedState) {
                this.selectedState = undefined;
            }
            else {
                this.selectedState = state;
            }
        },
        mouseover(state) {
            if (this.selectedState) {
                return;
            }
            console.log('mouseover no', state)
        }
    },
}
</script>

<style>
path {
    fill: #cad9ff;
    stroke: #6584d0;
    transition: fill .2s ease-in-out, stroke .2s ease-in-out;
}

path:hover {
    fill: #5279da;
    stroke: #a4bfff;
}
</style>