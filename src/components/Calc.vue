<template>
  <div id="blur"></div>
  <div id="calc-background">
    <div id="oldresult">6000/2+3227*2</div>
    <div id="calculating">100+10</div>
    <button id="e">e</button>
    <button id="micro"><span>&#181;</span></button>
    <button id="sin">sin</button>
    <button id="deg">deg</button>
  </div>
</template>

<script setup lang="ts">

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url('https://fonts.googleapis.com/css?family=Poppins');
body{
  background-color: #DAF0FF;
  font-family: 'Poppins';
};
#blur{
  position: absolute;
  width: 357px;
  height: 835px;
  left: 639px;
  top: 164px;

  background: rgba(96, 190, 255, 0.55);
  filter: blur(123px);
  border-radius: 39px;
  z-index: 1;
}
#calc-background{
  position: absolute;
  width: 375px;
  height: 812px;
  left: 533px;
  top: 134px;
  background: #F7F8FB;
  backdrop-filter: blur(102px);

  border-radius: 39px;
  z-index: 2;
}
#oldresult{
  position: absolute;
width: 175px;
height: 36px;
left: 167px;
top: 138px;

font-family: 'Poppins';
font-style: normal;
font-weight: 400;
font-size: 24px;
line-height: 36px;



color: #818181;
}
#calculating{
  position: absolute;
  width: 171px;
  height: 72px;
  left: 171px;
  top: 180px;

  font-family: 'Poppins';
  font-style: normal;
  font-weight: 500;
  font-size: 48px;
  line-height: 72px;
/* identical to box height */


  color: #424242;
}
#e{
  box-sizing: border-box;

/* Auto layout */

display: flex;
flex-direction: column;
justify-content: center;
align-items: center;
padding: 6px 4px;
gap: 10px;

  position: absolute;
  width: 62px;
  height: 40px;
  left: 34px;
  top: 330px;

  background-color: #FFFFFF;
  border: 1px solid #FFFFFF;
  backdrop-filter: blur(12px);
/* Note: backdrop-filter has minimal browser support */

  border-radius: 16px;
  color: #7CC9FF;
}
#micro{
  box-sizing: border-box;

/* Auto layout */

display: flex;
flex-direction: column;
justify-content: center;
align-items: center;
padding: 6px 4px;
gap: 10px;

position: absolute;
width: 62px;
height: 40px;
left: 116px;
top: 330px;

background: #FFFFFF;
border: 1px solid #FFFFFF;
backdrop-filter: blur(12px);
/* Note: backdrop-filter has minimal browser support */

border-radius: 16px;
color: #7CC9FF;
}
#sin{
  box-sizing: border-box;

/* Auto layout */

display: flex;
flex-direction: column;
justify-content: center;
align-items: center;
padding: 6px 4px;
gap: 10px;

position: absolute;
width: 62px;
height: 40px;
left: 198px;
top: 330px;

background: #FFFFFF;
border: 1px solid #FFFFFF;
backdrop-filter: blur(12px);
/* Note: backdrop-filter has minimal browser support */

border-radius: 16px;
color: #7CC9FF;
}
#deg{
/* Frame 28 */


box-sizing: border-box;

/* Auto layout */

display: flex;
flex-direction: column;
justify-content: center;
align-items: center;
padding: 6px 4px;
gap: 10px;

position: absolute;
width: 62px;
height: 40px;
left: 280px;
top: 330px;

background: #FFFFFF;
border: 1px solid #FFFFFF;
backdrop-filter: blur(12px);
/* Note: backdrop-filter has minimal browser support */

color: #7CC9FF;
/* Note: backdrop-filter has minimal browser support */

border-radius: 16px;
}
#ac{
  box-sizing: border-box;

/* Auto layout */

display: flex;
flex-direction: column;
justify-content: center;
align-items: center;
padding: 6px 4px;
gap: 10px;

position: absolute;
width: 62px;
height: 62px;
left: 34px;
top: 386px;

background: #FFFFFF;
border: 1px solid #FFFFFF;
backdrop-filter: blur(12px);
/* Note: backdrop-filter has minimal browser support */
color: #7CC9FF;
border-radius: 16px;
}
#back{
  
position: absolute;
width: 62px;
height: 62px;
left: 116px;
top: 386px;

background: linear-gradient(129.7deg, rgba(255, 255, 255, 0.6) -9.69%, rgba(255, 255, 255, 0.4) 114.23%);
border-radius: 16px;

border-radius: 16px;
}
#divide{
  position: absolute;
width: 62px;
height: 62px;
left: 198px;
top: 386px;

background: #ADE2FF;
border-radius: 12px;
color:#109DFF;
}
</style>
