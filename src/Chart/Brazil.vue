<template>
    <svg width="798" height="756" viewBox="0 0 798 756" fill="none" xmlns="http://www.w3.org/2000/svg">
        <AC @click.native="select('AC')" />
        <AL @click.native="select('AL')" />
        <AM @click.native="select('AM')" />
        <AP @click.native="select('AP')" />
        <BA @click.native="select('BA')" />
        <CE @click.native="select('CE')" />
        <DF @click.native="select('DF')" />
        <ES @click.native="select('ES')" />
        <GO @click.native="select('GO')" />
        <MA @click.native="select('MA')" />
        <MG @click.native="select('MG')" />
        <MS @click.native="select('MS')" />
        <MT @click.native="select('MT')" />
        <PA @click.native="select('PA')" />
        <PB @click.native="select('PB')" />
        <PE @click.native="select('PE')" />
        <PI @click.native="select('PI')" />
        <PR @click.native="select('PR')" />
        <RJ @click.native="select('RJ')" />
        <RN @click.native="select('RN')" />
        <RO @click.native="select('RO')" />
        <RR @click.native="select('RR')" />
        <RS @click.native="select('RS')" />
        <SC @click.native="select('SC')" />
        <SE @click.native="select('SE')" />
        <SP @click.native="select('SP')" />
        <TO @click.native="select('TO')" />
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
    methods: {
        select(state) {
            console.log('Clicou no ', state)
        }
    },
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
    }
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