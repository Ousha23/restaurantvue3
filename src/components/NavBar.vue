<template>
    <nav>
        <ul id="logo">
            <li>La tulipe</li>
        </ul>
        <ul id="nav">
            <li>ACCUEIL</li>
            <li>A PROPOS</li>
            <li>MENU</li>
            <li id="reserve">RESERVER MAINTENANT</li>
        </ul>
    </nav>
</template>

<style scoped>
    
nav {
    gap: 10px;
    display: flex;
    justify-content: space-between;
    margin-top: 0;
    padding: 10px;
    position: fixed;
    top: 0;
    width: 100%;
    z-index: 2;
}

#logo {
    font-family: 'Cake';
    list-style-type: none;
    padding: 0;
    font-size: 100px;
}

#nav{
    font-family: 'Lemon';
    align-content: end;
    text-align: center;
    list-style-type: none;
    display: flex;
    gap: 30px;
    justify-content: space-around;
    align-items: center;
    background-color: rgba(21, 20, 19, 0.377);
    position: relative;
    padding: 10px;
}

#triangleLi {
    width: 0px;
    height: 0px;
    border-style: solid;
    border-width: 0 0 100px 100px;
    border-color: transparent transparent rgba(21, 20, 19, 0.377) transparent;
    transform: rotate(360deg);

}
#reserve {
    border-color: burlywood;
    color: burlywood;
    border-style: double;
    padding: 10px;
}
</style>