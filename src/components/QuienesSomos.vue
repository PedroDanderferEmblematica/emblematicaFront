<template>
    <section id="QuienesSomos">
        <div></div>
        <div>
            <h2>Potencia tu marca con productos personalizados a medida</h2>
            <p>
                Destaca en un mercado saturado y construye una identidad de marca única. En nuestra empresa, 
                entendemos tu necesidad de productos y elementos personalizados que reflejen tu esencia. Nosotros lo resolvemos.
            </p>
            <p>
                Potencia tu marca con nuestra exclusiva personalización. Nuestro equipo de expertos está listo para ayudarte a llevar 
                tu identidad de marca al siguiente nivel. ¡Contáctanos ahora y descubre cómo podemos cerrar la brecha entre tu visión y 
                la realidad!
            </p>
            <ul>
                <li>
                    <div>
                        <img src="#" alt="#"/>
                        <h3>Diferenciación estratégica</h3>
                        <p>Sobresale de la competencia y capta la atención de tus clientes con una imagen coherente y distintiva en todos tus productos</p>
                    </div>
                </li>
                <li>
                    <div>
                        <img src="#" alt="#"/>
                        <h3>Mayor visibilidad</h3>
                        <p>Haz que tu marca esté presente constantemente en la mente de tus clientes a través de productos personalizados que llevan tu mensaje.</p>
                    </div>
                </li>
                <li>
                    <div>
                        <img src="#" alt="#"/>
                        <h3>Fidelización de clientes</h3>
                        <p>Crea una conexión emocional duradera con tus clientes, mostrándoles que valoras su relación y te preocupas por su experiencia.</p>
                    </div>
                </li>
                <li>
                    <div>
                        <img src="#" alt="#"/>
                        <h3>Adaptación precisa</h3>
                        <p>Nos ajustamos a tus necesidades específicas, desde materiales y colores hasta diseño y funcionalidad, para crear productos que representen tu marca a la perfección.</p>
                    </div>
                </li>
            </ul>
        </div>
    </section>
</template>

<style>
    #QuienesSomos{
        width: 100%;
        display: grid;
        grid-template-columns: 1fr;
        grid-template-rows: 200px 1fr;
    }

    #QuienesSomos >div:first-of-type{
        background-color: yellowgreen;
    }

    #QuienesSomos >div:last-of-type{
        padding: 10px;
    }

    #QuienesSomos >div:last-of-type >h2{
        width: 100%;
    }

    #QuienesSomos >div:last-of-type >p{
        margin-top: 10px;
    }

    #QuienesSomos >div:last-of-type >ul{
        display: grid;
        grid-template-columns: 1fr;
        grid-template-rows: 1fr 1fr 1fr 1fr;
        list-style: none;
        margin-top: 10px;
    }

    #QuienesSomos >div:last-of-type >ul >li{
        width: 100%;
        height: fit-content;
    }

    #QuienesSomos >div:last-of-type >ul >li >div{
        display: grid;
        grid-template-columns: 1fr;
        grid-template-rows: 70px auto auto;
        text-align: center;
    }

    #QuienesSomos >div:last-of-type >ul >li >div >img{
        width: 70px;
        height: 70px;
        background-color: blue;
        display: flex;
        align-self: center;
        justify-self: center;
    }

    #QuienesSomos >div:last-of-type >ul >li >div >h3{
        margin-top: 10px;
    }

    #QuienesSomos >div:last-of-type >ul >li >div >p{
        font-size: 14px;
    }

    @media (min-width:600px){

        #QuienesSomos{
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }

        #QuienesSomos >div:last-of-type >ul{
            grid-template-columns: 1fr 1fr;
            grid-template-rows: 1fr 1fr;
            grid-gap: 20px;
        }
    }

    @media (min-width:900px){

        #QuienesSomos{
            max-width: 900px;
            grid-template-columns: 300px 1fr;
            grid-template-rows: 1fr;
            padding-top: 20px;
            grid-gap: 20px;
        }

        #QuienesSomos >div:last-of-type{
            padding: 0;
        }

        #QuienesSomos >div:last-of-type >h2{
            font-size: 30px;
        }
    }
</style>