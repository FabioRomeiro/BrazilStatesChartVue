<script setup>
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
import { ref, shallowRef } from 'vue'

const selectedState = ref(null)

const stateComponents = shallowRef([
    {...AC, name: 'AC' },
    {...AL, name: 'AL' },
    {...AM, name: 'AM' },
    {...AP, name: 'AP' },
    {...BA, name: 'BA' },
    {...CE, name: 'CE' },
    {...DF, name: 'DF' },
    {...ES, name: 'ES' },
    {...GO, name: 'GO' },
    {...MA, name: 'MA' },
    {...MG, name: 'MG' },
    {...MS, name: 'MS' },
    {...MT, name: 'MT' },
    {...PA, name: 'PA' },
    {...PB, name: 'PB' },
    {...PE, name: 'PE' },
    {...PI, name: 'PI' },
    {...PR, name: 'PR' },
    {...RJ, name: 'RJ' },
    {...RN, name: 'RN' },
    {...RO, name: 'RO' },
    {...RR, name: 'RR' },
    {...RS, name: 'RS' },
    {...SC, name: 'SC' },
    {...SE, name: 'SE' },
    {...SP, name: 'SP' },
    {...TO, name: 'TO' },
])

function onClick (state) {
    selectedState.value = state === selectedState.value ? null : state
}

function onMouseOver (state) {
    if (selectedState.value) {
        return
    }
    console.log('mouseover no', state)
}
</script>

<template>
    <svg width="798" height="756" viewBox="0 0 798 756" fill="none" xmlns="http://www.w3.org/2000/svg">
        <component
            v-for="state in stateComponents"
            :key="state.name"
            :is="state"
            @click.native="onClick(state.name)"
            @mouseover.native="onMouseOver(state.name)"
        />
    </svg>
</template>

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