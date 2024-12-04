<template>
    <main id="sectionTwo">
        <div>
            <div id="titles">
                <h3>TRADITION & INNOVATION</h3>
                <h2>DES TABLES D'EXCEPTION</h2>
            </div>
            <div id="detailYearsParent">
                <div id="detailYearsLeft">
                    <PressComp :title="'PREMIER RESTAURANT'" :year="'1955:'"/>
                    <PressComp :title="'OUVERTURE DE L\'HOTEL'" :year="'2005:'"/>
                </div>
                <div id="detailImg">
                    <img id="imgTable" src="@/assets/img/table.jpg" alt="photo table">
                </div>
                <div id="detailYearsRight">
                    <PressComp :title="'ETOILE MICHELIN'" :year="'1970:'"/>
                    <PressComp :title="'HERITAGE'" :year="'2022:'"/>
                </div>
            </div>
        </div>
    </main>
</template>

<style scoped>
    #sectionTwo {
        position: relative;
        overflow: hidden;
        padding-top: 30px;
        display: flex;
        width: 100%;
        justify-content: center;
        background-color: rgb(43, 43, 43);
    }

    #divDetails {
        display: flex;
        width: 100%;
    }

    img {
        width: 250px;
        height: 250px;
        border-radius: 50%;
    }

    #titles {
        width: 50%;
        text-align: center;
        justify-content: center;
        margin: auto;
    }

    h2 {
        font-size: xx-large;
        padding: 30px;
    }
    h3 {
        font-size: larger;
        color: burlywood;
        position: relative;
        width: 50%;
        margin: auto;
    }

    h3::after {
        content: '';
        height: 2px;
        width: 100%;
        position: absolute;
        bottom: 0px;
        right: 0;
        background: radial-gradient(burlywood, black);
    }

    #detailYearsParent {
        display: flex;
        padding: 30px;
        align-items: center;
    }

    #detailYearsLeft, #detailYearsRight, #detailImg {
        padding: 50px;
    }

    #detailYearsRight, #detailYearsLeft {
        padding: 10px;
    }
    #detailYearsLeft {
        text-align: right;
    }
</style>

<script setup>
    import PressComp from './PressComp.vue';
</script>