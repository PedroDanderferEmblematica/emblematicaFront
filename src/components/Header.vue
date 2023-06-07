<script>
  export default {
    methods:{
      displayMenu(){
      
        const d = document;

        let navMenu = d.getElementById('navMenu');

        if(navMenu.getBoundingClientRect().y < 0){
          navMenu.style.transform='translateY(0px)'
        }else{
          navMenu.style.transform='translateY(-100vh)'
        }
      }
    }
  }
</script>
<template>
  <header>
    <div>
      <h1>Emblematica</h1>
      <div>
        <button @click="displayMenu">
          <div>
            <span>Menú</span>
            <span></span>
            <span></span>
          </div>
        </button>
        <nav id="navMenu">
          <ul>
            <li><a href="#"><span>Quienes somos</span></a></li>
            <li><a href="#"><span>Trabajos</span></a></li>
            <li><a href="#"><span>Como trabajamos</span></a></li>          
            <li><a href="#"><span>Contactanos</span></a></li>
          </ul>
        </nav>
      </div>
    </div>
  </header>
</template>

<style>
  header{
  }

  header >div{
    display: grid;
    grid-template-columns: 1fr auto;
    grid-template-rows: 1fr;
    padding: 5px;
    height: 80px;
  }

  header >div >h1{
    background-color: brown;
    font-size: 0;
    width: 25vw;
    min-width: 80px;
    max-width: 110px;
    height: 15vw;
    min-height: 40px;
    max-height: 70px;
    display: flex;
    align-self: center;
    justify-self: flex-start;
  }

  header >div >div{
    display: grid;
    grid-template-columns: 1fr;
    grid-template-rows: 1fr;
  }

  header >div >div >button{
    height: 8vw;
    min-height: 40px;
    max-height: 50px;
    width: 8vw;
    min-width: 40px;
    max-width: 50px;
    font-size: 0;
    border: 0;
    display: flex;
    align-self: center;
    justify-self: center;
    background-color: #fff;
  }

  header >div >div >button >div{
    display: grid;
    grid-template-columns: 1fr;
    grid-template-rows: 1fr 3px 1fr;
    width: 100%;
  }
  header >div >div >button >div >span{
    display: flex;
    align-self: center;
    justify-self: center;
    width: 100%;
    height: 3px;
    background-color: #333;
    border: 1px sokid #333;
    border-radius: 50px;
  }

  header >div >div >nav{
    position: absolute;
    top: 80px;
    left: 0;
    width: 100vw;
    height: fit-content;
    transform: translateY(-100vh);
    transition: 1s;
    background-color: white;
  }

  header >div >div >nav >ul{
    display: grid;
    grid-template-columns: 1fr;
    grid-template-rows: 1fr 1fr 1fr 1fr;
    grid-gap: 5px;
    padding-top: 5px;
    list-style: none;
  }

  header >div >div >nav >ul >li >a{
    font-size: 20px;
    display: grid;
    grid-template-columns: 1fr;
    grid-template-rows: 1fr;
    text-decoration: none;
    color: black;
    padding: 5px;
    height: 60px;
  }

  header >div >div >nav >ul >li >a >span{
    display: flex;
    align-self: center;
    justify-self: flex-start;
  }

  @media (min-width:900px){
    header{
      max-width: 1100px;
      margin-left: auto;
      margin-right: auto;
    }
    header >div >div >button{
      display: none;
    }
    header >div >div >nav{
      position: unset;
      top: unset;
      left: unset;
      width: 100%;
      height: fit-content;
      transform: none;
      align-self: center;
      justify-self: center;
    }
  
    header >div >div >nav >ul{
      grid-template-columns: 1fr 1fr 1fr 1fr;
      grid-template-rows: 1fr;
      padding-top: 0;
    }
  
    header >div >div >nav >ul >li >a >span{
      justify-self: center;
    }
  }
</style>