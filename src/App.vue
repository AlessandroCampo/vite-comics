

<template>
    <DcHeader></DcHeader>
    <main>
        ...Content goes here...
    </main>
    <section>
        <DcNavbar></DcNavbar>
    </section>
    <DcFooter></DcFooter>
</template>



<script>

import DcHeader from '../src/components/DcHeader.vue';
import DcNavbar from '../src/components/DcNavbar.vue';
import DcFooter from '../src/components/DcFooter.vue';

export default {
    components: {
        DcHeader,
        DcNavbar,
        DcFooter
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

main {
    color: white;
    font-size: 40px;
    margin-block: 30px;
    text-align: center;
}
</style>