<script>
import axios from 'axios';
  export default {
    methods:{
        showError(){
            console.log('error');
        },
        formSubmit(req){

            let name = req.target[0].value, email = req.target[1].value, content = req.target[2].value;

           
        
                axios.post('https://emblematicabackok.uc.r.appspot.com/', {
                    name: name,
                    email: email,
                    content: content
                })
                .then(function (response) {
                    console.log(response);
                })
                .catch(function (error) {
                    console.log(error);
                });
            
        }
    }
}
</script>
<template>
    <section id="Contactanos">
        <h2>Contactate con nosotros</h2>
        <div>
            <div>
                <a href="#"><div><div><span></span><span>Escribinos un whatsapp</span></div></div></a>
                <ul>
                    <li><a href="#"><div><div><span></span><span>Instagram</span></div></div></a></li>
                    <li><a href="#"><div><div><span></span><span>LinkedIn</span></div></div></a></li>
                </ul>
                <ul>
                    <li><span>Número de teléfono: </span><span>+54 9 11 6666-6666</span></li>
                    <li><span>Correo electronico: </span><span>consultas@emblematica.ar</span></li>
                </ul>
            </div>
            <div>
                <h3>Envianos un mensaje</h3>
                <form action="#" method="POST" @submit.prevent="formSubmit">
                    <div>
                        <input type="text" name="nombre" placeholder="Nombre">
                    </div>
                    <div>
                        <input type="text" name="email" placeholder="Correo electronico">
                    </div>
                    <div>
                        <textarea name="comentario" id="" cols="30" rows="10" placeholder="Dejanos tu comentario"></textarea>
                    </div>
                    <input type="submit" value="Enviar">
                </form>
            </div>
        </div>
    </section>
</template>
<style>
    #Contactanos{
        padding: 20px 10px 10px 10px;
    }

    #Contactanos >div{
        margin-top: 10px;
        display: grid;
        grid-template-columns: 1fr;
        grid-template-rows: 1fr auto;
        grid-gap: 5px;
    }

    #Contactanos >div >div:first-of-type{
        display: grid;
        grid-template-columns: 1fr;
        grid-template-rows: 1fr 1fr;
    }
    #Contactanos >div >div:first-of-type >a{
        display: block;
        width:100%;
        background-color: #25d366;
        border: 1px solid #25d366;
        border-radius: 500px;
        text-align: center;
        text-decoration: none;
        color: black;
        height: 40px;
        display: grid;
        grid-template-columns: 1fr;
        grid-template-rows: 1fr;

    }

    #Contactanos >div >div:first-of-type >a >div{
        display: flex;
        align-self: center;
        justify-self: center;
        width: fit-content;
        height: fit-content;
    }
    #Contactanos >div >div:first-of-type >a >div >div{
        display: grid;
        grid-template-columns: 25px 1fr;
        grid-template-rows: 1fr;
        grid-gap: 5px;
    }

    #Contactanos >div >div:first-of-type >a >div >div >span:first-of-type{
        display: block;
        width: 25px;
        height: 25px;
        background-image: url('../assets/img/whatsapp_logo.png');
        background-size: contain;
        background-position: center;
        background-repeat: no-repeat;
        display: flex;
        align-self: center;
        justify-self: center;
    }

    #Contactanos >div >div:first-of-type >a >div >div >span:last-of-type{
        display: flex;
        align-self: center;
        justify-self: center;
        color: white;
    }

    #Contactanos >div >div:first-of-type >ul:first-of-type{
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-template-rows: 1fr;
        list-style: none;
        margin-top: 10px;
    }
    #Contactanos >div >div:first-of-type >ul:first-of-type >li{
        height: 40px;
        border: 1px solid transparent #333;
        text-align: center;
        display: flex;
        
    }

    #Contactanos >div >div:first-of-type >ul:first-of-type >li:first-of-type{
        border-top-left-radius: 500px;
        border-bottom-left-radius: 500px;
        background: #f09433; 
        background: -moz-linear-gradient(45deg, #f09433 0%, #e6683c 25%, #dc2743 50%, #cc2366 75%, #bc1888 100%); 
        background: -webkit-linear-gradient(45deg, #f09433 0%,#e6683c 25%,#dc2743 50%,#cc2366 75%,#bc1888 100%); 
        background: linear-gradient(45deg, #f09433 0%,#e6683c 25%,#dc2743 50%,#cc2366 75%,#bc1888 100%); 
        filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#f09433', endColorstr='#bc1888',GradientType=1 );
    }

    #Contactanos >div >div:first-of-type >ul:first-of-type >li:last-of-type{
        background: #0e76a8; 
        border-top-right-radius: 500px;
        border-bottom-right-radius: 500px;
    }

    #Contactanos >div >div:first-of-type >ul:first-of-type >li >a{
        width: 100%;
        display: grid;
        grid-template-columns: 1fr;
        grid-template-rows: 1fr;
        text-decoration: none;
        color: white;
        font-weight: 700;
    }

    #Contactanos >div >div:first-of-type >ul:first-of-type >li >a >div{
        height: fit-content;
        width: fit-content;
        display: flex;
        align-self: center;
        justify-self: center;
    }
    #Contactanos >div >div:first-of-type >ul:first-of-type >li >a >div >div{
        display: grid;
        grid-template-columns: 20px 1fr;
        grid-template-rows: 1fr;
        grid-gap: 5px;
    }

    #Contactanos >div >div:first-of-type >ul:first-of-type >li >a >div >div >span:first-of-type{
        background-color: transparent;
        width: 20px;
        height: 20px;
        background-size: contain;
        background-repeat: no-repeat;
        background-position: center;
    }

    #Contactanos >div >div:first-of-type >ul:first-of-type >li >a >div >div >span:last-of-type{
        display: flex;
        align-self: center;
        justify-self: center;
    }

    #Contactanos >div >div:first-of-type >ul:first-of-type >li:first-of-type >a >div >div >span:first-of-type{
        background-image: url('../assets/img/instagram_logo.png');
    }

    #Contactanos >div >div:first-of-type >ul:first-of-type >li:last-of-type >a >div >div >span:first-of-type{
        background-image: url('../assets/img/linkedIn_logo.png');
    }

    #Contactanos >div >div:first-of-type >ul:last-of-type{
        display: grid;
        grid-template-columns: 1fr;
        grid-template-rows: 1fr 1fr;
        list-style: none;
        margin-top: 20px;
        grid-gap: 5px;
        padding: 0 5px 0 5px;
    }

    #Contactanos >div >div:first-of-type >ul:last-of-type >li{
        display: flex;
        display: grid;
        grid-template-columns: 20px 1fr;
        grid-template-rows: 1fr;
        grid-gap: 5px;
    }

    #Contactanos >div >div:first-of-type >ul:last-of-type >li >span:first-of-type{
        font-size: 0;
        width: 20px;
        height: 20px;
        background-size: contain;
        background-repeat: no-repeat;
        background-position: center;
    }

    #Contactanos >div >div:first-of-type >ul:last-of-type >li >span:last-of-type{
        display: flex;
        align-self: center;
        justify-self: flex-start;
        font-weight: 700;
    }
    #Contactanos >div >div:first-of-type >ul:last-of-type >li:first-of-type >span:first-of-type{
        background-image: url('../assets/img/telephone_icon.png');
    }
    #Contactanos >div >div:first-of-type >ul:last-of-type >li:last-of-type >span:first-of-type{
        background-image: url('../assets/img/email_icon.png');
    }

    #Contactanos >div >div:last-of-type{
        margin-top: 20px;
    }

    #Contactanos >div >div:last-of-type >form{
        display: grid;
        grid-template-columns: 1fr;
        grid-template-rows: 1fr 1fr auto 1fr;
        grid-gap: 10px;
        margin-top: 10px;
    }

    #Contactanos >div >div:last-of-type >form >div >input[type=text]{
        width: 100%;
        border: none;
        border-bottom: 1px solid #333;
        background-color: transparent;
        padding: 5px;
        outline: none;
    }

    #Contactanos >div >div:last-of-type >form >div >textarea{
        width: 100%;
        border: 1px solid #333;
        border-radius: 5px;
        background-color: transparent;
        padding: 5px;
        outline: none;
        resize: none;
    }

    #Contactanos >div >div:last-of-type >form >input[type=submit]{
        width: 100%;
        height: 40px;
        background-color: #0e76a8;
        border-radius: 5000px;
        color: white;
    }

    @media (min-width: 900px){
        #Contactanos{
            max-width: 900px;
            margin-left: auto;
            margin-right: auto;
        }

        #Contactanos >div{
            grid-template-columns: 1fr 1fr;
            grid-template-rows: 1fr;
            grid-gap: 20px;
        } 

        #Contactanos >div >div:first-of-type{
            height: fit-content;
        }

        #Contactanos >div >div:last-of-type{
            margin-top: 0;
        }
    }
</style>