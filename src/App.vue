

<template>
    <DcHeader></DcHeader>
    <main>
        ...Content goes here...
    </main>
    <section>
        <DcNavbar></DcNavbar>
    </section>
    <DcFooter></DcFooter>
    <DcSocials></DcSocials>
</template>



<script>

import DcHeader from '../src/components/DcHeader.vue';
import DcNavbar from '../src/components/DcNavbar.vue';
import DcFooter from '../src/components/DcFooter.vue';
import DcSocials from '../src/components/DcSocials.vue';

export default {
    components: {
        DcHeader,
        DcNavbar,
        DcFooter,
        DcSocials
    },
    data() {
        return {

        }
    },
    methods: {

    }
}

</script>


<style lang="scss">
@use './styles/general.scss';
@use './styles/partials/variables' as *;

main {
    color: white;
    font-size: 40px;
    margin-block: 42px;
    text-align: center;
    background-color: $dc_background;
}
</style>