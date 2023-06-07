<template>
    <section id="Contactanos">
        <h2>Contactate con nosotros</h2>
        <div>
            <a href="#">Escribinos un whatsapp</a>
            <ul>
                <li><a href="#"><div><span></span><span>Instagram</span></div></a></li>
                <li><a href="#">LinkedIn</a></li>
            </ul>
            <ul>
                <li><span>Número de teléfono: </span><span>+54 9 11 6666-6666</span></li>
                <li><span>Correo electronico: </span><span>consultas@emblematica.ar</span></li>
            </ul>
        </div>
        <form action="#" method="POST">
            <input type="text" name="nombre">
            <input type="text" name="email">
            <textarea name="comentario" id="" cols="30" rows="10"></textarea>
            <input type="submit" value="Enviar">
        </form>
    </section>
</template>
<style>
    #Contactanos{
        padding-top: 20px;
    }

    #Contactanos h2{
        margin-left: 10px;
    }

    #Contactanos >div{
        padding: 10px;
        display: grid;
        grid-template-columns: 1fr;
        grid-template-rows: 1fr 1fr;
    }
    #Contactanos >div >a{
        display: block;
        width:100%;
        background-color: greenyellow;
        border: 1px solid greenyellow;
        border-radius: 500px;
        text-align: center;
        text-decoration: none;
        color: black;
        height: 40px;
    }

    #Contactanos >div >ul:first-of-type{
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-template-rows: 1fr;
        list-style: none;
        margin-top: 10px;
    }
    #Contactanos >div >ul:first-of-type >li{
        height: 40px;
        border: 1px solid transparent #333;
        text-align: center;
        display: flex;
        
    }

    #Contactanos >div >ul:first-of-type >li:first-of-type{
        border-top-left-radius: 500px;
        border-bottom-left-radius: 500px;
        background: #f09433; 
        background: -moz-linear-gradient(45deg, #f09433 0%, #e6683c 25%, #dc2743 50%, #cc2366 75%, #bc1888 100%); 
        background: -webkit-linear-gradient(45deg, #f09433 0%,#e6683c 25%,#dc2743 50%,#cc2366 75%,#bc1888 100%); 
        background: linear-gradient(45deg, #f09433 0%,#e6683c 25%,#dc2743 50%,#cc2366 75%,#bc1888 100%); 
        filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#f09433', endColorstr='#bc1888',GradientType=1 );
    }

    #Contactanos >div >ul:first-of-type >li:last-of-type{
        background: #0e76a8; 
        border-top-right-radius: 500px;
        border-bottom-right-radius: 500px;
    }

    #Contactanos >div >ul:first-of-type >li >a{
        background-color: brown;
        width: 100%;
        display: grid;
        grid-template-columns: 1fr;
        grid-template-rows: 1fr;
        text-decoration: none;
        color: black;
    }

    #Contactanos >div >ul:first-of-type >li >a >div{
        height: fit-content;
        width: fit-content;
        display: flex;
        align-self: center;
        justify-self: center;
    }

    #Contactanos >div >ul:last-of-type{
        display: grid;
        grid-template-columns: 1fr;
        grid-template-rows: 1fr 1fr;
        list-style: none;
        margin-top: 10px;
        grid-gap: 5px;
        padding: 0 5px 0 5px;
    }

    #Contactanos >div >ul:last-of-type >li{
        display: flex;
        display: grid;
        grid-template-columns: 20px 1fr;
        grid-template-rows: 1fr;
        grid-gap: 5px;
    }

    #Contactanos >div >ul:last-of-type >li >span:first-of-type{
        font-size: 0;
        width: 20px;
        height: 20px;
        background-size: contain;
        background-repeat: no-repeat;
        background-position: center;
    }

    #Contactanos >div >ul:last-of-type >li >span:last-of-type{
        display: flex;
        align-self: center;
        justify-self: flex-start;
        font-weight: 700;
    }
    #Contactanos >div >ul:last-of-type >li:first-of-type >span:first-of-type{
        background-image: url('../assets/img/telephone_icon.png');
    }
    #Contactanos >div >ul:last-of-type >li:last-of-type >span:first-of-type{
        background-image: url('../assets/img/email_icon.png');
    }
</style>