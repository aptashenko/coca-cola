<template>
    <div class="container">
        <header class="content__header">
            <h1 class="content__title">FAI UNA PAUSA E GIOCA <span>CON</span></h1>
            <img src="../assets/images/logo.png" class="content__logo" />
        </header>
        
        <main class="content__body">
            <h2 class="content__subtitle">PUOI VINCERE SUBITO FINO A 100€ IN</h2>
            <p class="content__bottomTitle">Buoni Regalo Amazon.it**</p>
            <div class="content__card--wrapper">
                <img class="content__card" src="../assets/images/award_amazon.png" />
            </div>
            <p class="content__text">o altri fantastici premi!</p>
            <div class="content__rewards">
                <span class="right"><img class="content__rewardCola" src="../assets/images/header_step_1_mob.png" /></span>
                <span class="left"><img class="content__rewardCassa" src="../assets/images/header_step_2_mob.png" /></span>
            </div>
            <img class="content__spinner" src="../assets/images/header_left_mob.png" />
            <a class="content__button" href="#">GIOCA SUBITO</a>
        </main>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
.content {
    width: 100%;
    padding-bottom: 30px;

    &__header {
        height: fit-content;
        position: relative;
    }

    &__title {
        margin: 0;
        font-size: 38px;
        font-family: 'UnityCondensed Bold';
        text-transform: uppercase;
        color: #fff;
        display: flex;
        flex-direction: column;
        text-align: center;
        line-height: 1.5;

        & span {
            margin-left: 40px;
            width: fit-content;
        }
    }

    &__logo {
        width: 165px;
        position: absolute;
        top: 55px;
        left: 105px;
    }

    &__body {
        margin-top: 30px;
    }

    &__subtitle,
    &__bottomTitle,
    &__text {
        font-family: 'UnityCondensed Bold';
        text-align: center;
        font-size: 20px;
        margin: 0;
        color: #fff;
    }

    &__subtitle {
        font-size: 40px;
        color: #fff;
        line-height: 1;
    }

    &__bottomTitle {
        font-size: 38px;
    }

    &__text {
        text-transform: uppercase;
        font-size: 40px;
        line-height: 1;
    }

    &__card {
        display: block;
        margin: 0 auto;
        width: 250px;

        &--wrapper {
            position: relative;
            margin-top: 20px;

            &::before {
                content: '';
                width: 60px;
                height: 60px;
                top: 20px;
                left: 5px;
                position: absolute;
                background: url('../assets/images/stars_top_left.png');
                background-size: contain;
                background-repeat: no-repeat;
            }
        }
    }

    &__rewards {
        margin-top: 30px;
        display: flex;
        flex-direction: column;
        align-items: center;
        position: relative;

        & .right {
            &::before {
                content: '';
                width: 60px;
                height: 60px;
                right: 0;
                position: absolute;
                background: url('../assets/images/stars_right.png');
                background-repeat: no-repeat;
                background-size: contain;
            }
        }

        & .left {
            &::before {
                content: '';
                width: 60px;
                height: 60px;
                left: 0;
                top: 50%;
                position: absolute;
                background: url('../assets/images/stars_right.png');
                background-repeat: no-repeat;
                background-size: contain;
            }
        }
    }

    &__rewardCola {
        width: 130px;
    }

    &__rewardCassa {
        margin-top: 30px;
        width: 200px;
    }

    &__spinner {
        width: 300px;
        display: block;
        margin: 20px auto 0;
    }

    &__button {
        color: #be1322;
        font-family: 'UnityCondensed Bold';
        font-size: 30px;
        letter-spacing: 1px;
        background: #fff;
        border-radius: 15px;
        padding: 5px 0;
        max-width: 280px;
        margin: 10px auto 0;
        text-align: center;
        display: block;
        border: none;
        text-decoration: none;
    }
}
@media screen and (min-width: 768px) {
    .content {
        padding-bottom: 60px;

        &__title {
            font-size: 100px;
        }

        &__logo {
            width: 400px;
            top: 150px;
            left: 200px;
        }

        &__subtitle,
        &__bottomTitle {
            font-size: 87px;
        }

        &__card {
            width: 500px;

            &--wrapper {
                &::before {
                    width: 120px;
                    height: 120px;
                    top: 40px;
                    left: 25px;
                }
            }
        }

        &__text {
            font-size: 90px;
        }

        &__rewards {

            & .left,
            & .right {
                &::before {
                    width: 90px;
                    height: 90px;
                }
            }
        }

        &__rewardCola {
            width: 250px;
        }

        &__rewardCassa {
            width: 370px;
        }

        &__spinner {
            width: 660px;
        }

        &__button {
            max-width: 660px;
            font-size: 68px;
            margin-top: 30px;
            border-radius: 30px;
        }
    }
}
</style>