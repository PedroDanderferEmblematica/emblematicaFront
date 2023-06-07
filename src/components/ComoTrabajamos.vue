<template>
    <section id="ComoTrabajamos">
        <h2>¿Como trabajamos?</h2>
        <ol>
            <li>
                <div>
                    <img src="#" alt="#">
                    <h3>Comunicanos tu idea</h3>
                    <p>Contanos que estas buscando, en Emblemática vamos ayudarte a realizar un producto final único.</p>
                </div>
            </li>
            <li>
                <div>
                    <img src="#" alt="#">
                    <h3>Diseñamos el producto final</h3>
                    <p>Realizamos muestras para que veas y apruebes el producto final.</p>
                </div>
            </li>
            <li>
                <div>
                    <img src="#" alt="#">
                    <h3>Definimos la entrega</h3>
                    <p>Planteamos las fechas de entrega y de pagos, nos ajustamos a tus necesidades.</p>
                </div>
            </li>
            <li>
                <div>
                    <img src="#" alt="#">
                    <h3>Mostra tu marca al mundo</h3>
                    <p>Expone tu marca para que todos la conozcan</p>
                </div>
            </li>
        </ol>
    </section>
</template>

<style>
    #ComoTrabajamos{
        padding-top: 20px;
    }

    #ComoTrabajamos h2{
        margin-left: 10px;
    }

    #ComoTrabajamos >ol{
        display: grid;
        grid-template-columns: 1fr;
        grid-template-rows: 1fr 1fr 1fr 1fr;
        grid-gap: 10px;
        margin-top: 20px;
    }

    #ComoTrabajamos >ol >li{
        display: flex;
        align-self: center;
        justify-self: center;
        max-width: 400px;
    }

    #ComoTrabajamos >ol >li >div{
        display: grid;
        grid-template-columns: 1fr;
        grid-template-rows: 1fr auto auto;
        text-align: center;
    }

    #ComoTrabajamos >ol >li >div >img{
        width: 80px;
        height: 80px;
        background-color: blue;
        display: flex;
        align-self: center;
        justify-self: center;
        
    }

    #ComoTrabajamos >ol >li >div >h3{
        margin-top: 10px;
        font-weight: 400;
    }

    #ComoTrabajamos >ol >li >div >p{
        width: 80%;
        margin-left: auto;
        margin-right: auto;
    }

    @media (min-width:600px){

        #ComoTrabajamos{
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }

    }

    @media (min-width:900px){

        #ComoTrabajamos{
            max-width: 900px;
            padding-top: 40px;
        }

        #ComoTrabajamos >ol{
            grid-template-columns: 1fr 1fr 1fr 1fr;
            grid-template-rows: 1fr;
            padding-top: 20px;
        }

        #ComoTrabajamos >ol >li{
            align-self: flex-start;
            justify-self: center;
        }
    }
</style>