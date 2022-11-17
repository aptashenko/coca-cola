<template>
    <footer class="footer">
        <div class="container">
            <div class="footer__wrapper">
                <p class="footer__text">
                    *Concorso valido con l’acquisto di VAP 250ml, 275ml e 330ml, CAN 330ml, PET 400ml e 450ml.
                </p>
                <img class="footer__brands" src="../assets/images/brands.png" />
                <div>
                    <p class="footer__text">
                        **Restrizioni applicate. Vedere dettagli su: amazon.it/gc-legal.
                    </p>
                    <p class="footer__text">
                        Concorso valido dal 24.10.2022 al 28.02.2023. Stima montepremi € 32.650,00 + iva ove dovuta.
                    </p>
                    <p class="footer__text">
                        ©2022 The Coca-Cola Company. ©2022 DP Beverages UC. ©2022 SIBIL S.r.l.
                    </p>
                </div>
                <a class="footer__link" href="#" target="_blank">REGOLAMENTO</a>
            </div>
        </div>
    </footer>
</template>

<script>
export default {

}
</script>

<style lang="scss">
.footer {
    background: #fff;
    padding: 20px 0;
    font-family: 'HelveticaNeue';
    font-weight: bold;

    &__text {
        font-size: 10px;
        margin: 0;
        text-align: center;
    }

    &__brands {
        max-width: 100%;
        display: block;
        margin: 0 auto 10px;
        width: 200px;
    }

    &__link {
        display: block;
        text-align: center;
        font-size: 10px;
        margin-top: 10px;
        text-decoration: underline;
        color: #000;
    }
}

@media screen and (min-width: 768px) {
    .footer {

        &__text,
        &__link {
            font-size: 14px;
        }

        &__brands {
            width: 400px;
            margin: 10px auto 20px;
        }
    }
}

@media screen and (min-width: 1000px) {
    .footer {
        &__wrapper {
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        &__text, &__link {
            text-align: left;
            font-size: 11px;
        }

        &__brands {
            width: 250px;
            margin: 0;
            height: 50px;
        }
    }
}
</style>