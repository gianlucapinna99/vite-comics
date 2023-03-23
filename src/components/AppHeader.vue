<template>
    <section class="main-header">
        <div>
            <img src="../assets/img/dc-logo.png" alt="">
        </div>
        <div>
            <ul class="menu">
                <li>CHARACTERS</li>
                <li>COMICS</li>
                <li>MOVIES</li>
                <li>TV</li>
                <li>GAMES</li>
                <li>COLLECTIBLES</li>
                <li>VIDEOS</li>
                <li>FANS</li>
                <li>NEWS</li>
                <li>SHOP</li>
            </ul>
        </div>
    </section>
</template>


<style scoped>
.menu li {
    list-style: none;
}

.menu {
    display: flex;
    gap: 10px;
    font-weight: 700;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    font-size: 18px;
    align-items: center;
    height: 100%;
}

.main-header {
    height: 115px;
    display: flex;
    width: 80%;
    margin: 0 auto;
    justify-content: space-between;
    align-items: center;
}
</style>