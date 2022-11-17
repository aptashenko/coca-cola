<template>
  <div class="container">
    <header class="desktop__header">
        <h1 class="desktop__title">Fai una pausa E GIOCA con</h1>
        <img src="../assets/images/logo.png" class="desktop__logo" />
    </header>
    <main class="desktop__body">
        <img src="../assets/images/header_left.png" class="desktop__spinner" />
        <div class="desktop__description">
            <p class="desktop__text">PUOI VINCERE SUBITO FINO A 100€</p>
            <p class="desktop__text">IN Buoni Regalo Amazon.it**</p>
            <p class="desktop__text desktop__text--fontSize">o altri fantastici premi!</p>
        </div>
        <img src="../assets/images/award_amazon.png" class="desktop__card" />
        <div class="desktop__rewards">
            <img src="../assets/images/header_step_1.png" class="desktop__rewardCola" />
            <img src="../assets/images/header_step_2.png" class="desktop__rewardCassa" />
        </div>
        <a class="desktop__button" href="#">GIOCA SUBITO</a>
    </main>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
.desktop {
    &__header {
        display: flex;
        justify-content: center;
        align-items: center;
        margin-top: 20px;
    }
    &__title {
        display: inline;
        margin: 0;
        font-size: 80px;
        font-family: 'UnityCondensed Bold';
        text-transform: uppercase;
        color: #fff;
        text-align: center;
    }
    &__logo {
        width: 300px;
        margin-left: 15px;
    }

    &__body {
        position: relative;
        margin-top: 30px;
    }

    &__spinner {
        width: 460px;
        position: relative;
        top: -30px;
        left: 0;
    }

    &__description {
        position: absolute;
        top: -14px;
        left: 383px;
    }

    &__text {
        font-family: 'UnityCondensed Bold';
        text-align: center;
        font-size: 48px;
        line-height: 1;
        margin: 0;
        color: #fff;
        &--fontSize {
            margin-left: 30px;
            font-size: 55px;
            text-transform: uppercase;
        }
    }

    &__card {
        position: absolute;
        top: -45px;
        right: -50px;
        width: 300px;
    }

    &__rewards {
        display: flex;
        align-items: flex-start;
        width: fit-content;
        position: absolute;
        bottom: 129px;
        right: 0;
    }

    &__rewardCola {
        width: 280px;
    }

    &__rewardCassa {
        width: 330px;
    }

    &__button {
        color: #be1322;
        font-family: 'UnityCondensed Bold';
        font-size: 55px;
        letter-spacing: 1px;
        background: #fff;
        border-radius: 29px;
        padding: 5px 30px;
        margin: 0 auto;
        text-align: center;
        display: block;
        border: none;
        text-decoration: none;
        width: 420px;
        position: absolute;
        bottom: 0;
        right: 85px;
    }
}
</style>