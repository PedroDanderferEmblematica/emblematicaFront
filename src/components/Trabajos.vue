<template>
    <section id="Trabajos">
        <ul>
            <li><a href="#">Trabajo 1</a></li>
            <li><a href="#">Trabajo 1</a></li>
            <li><a href="#">Trabajo 1</a></li>
            <li><a href="#">Trabajo 1</a></li>
            <li><a href="#">Trabajo 1</a></li>
            <li><a href="#">Trabajo 1</a></li>
        </ul>
    </section>
</template>

<style>

 #Trabajos >ul{
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-template-rows: 1fr 1fr 1fr;
    list-style: none;
    width: 100%;
 }

 #Trabajos >ul >li{
    background-color: blue;
    width: 50vw;
    height: 50vw;
 }

 #Trabajos >ul >li >a{
    background-color: rgba(0,0,0,0.5);
    display: block;
    height: 50vw;
    width: 50vw;
    font-size: 0;
 }

 @media (min-width:600px){

    #Trabajos{
        max-width: 600px;
        margin-left: auto;
        margin-right: auto;
    }

    #Trabajos >ul >li{
        max-width: 300px;
        max-height: 300px;
     }

     #Trabajos >ul >li >a{
        max-width: 300px;
        max-height: 300px;
     }
}

@media(min-width:900px){

    #Trabajos{
        max-width: 900px;
        padding-top: 40px;
    }
    
    #Trabajos >ul{
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        grid-template-rows: 1fr 1fr;
        list-style: none;
     }
}

</style>