<template>
  <section class="preloader">
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
  </section>
</template>

<style lang="css" scoped>
section {
  height:100vh;
  background: #2A0E49;
}
div {
  background-image:url('@/assets/img/figure.png');
  background-size:contain;
  height:112px; width:105px;
  position:absolute;
  opacity:0.05;
  top:calc(50% - 66px);
  left:calc(50% - 66px);
  -webkit-animation:opacity 2s ease-in-out infinite;
  animation:opacity 2s ease-in-out infinite;
}
div:nth-child(-n+7):not(:nth-child(1)) { -webkit-animation:opacity 2s 0.25s ease-in-out infinite; animation:opacity 2s 0.25s ease-in-out infinite; }
div:nth-child(-n+19):not(:nth-child(-n+7)) { -webkit-animation:opacity 2s 0.5s ease-in-out infinite; animation:opacity 2s 0.5s ease-in-out infinite; }
div:nth-child(-n+37):not(:nth-child(-n+19)) { -webkit-animation:opacity 2s 0.75s ease-in-out infinite; animation:opacity 2s 0.75s ease-in-out infinite; }
div:nth-child(-n+61):not(:nth-child(-n+37)) { -webkit-animation:opacity 2s 1s ease-in-out infinite; animation:opacity 2s 1s ease-in-out infinite; }
div:nth-child(-n+79):not(:nth-child(-n+61)) { -webkit-animation:opacity 2s 1.25s ease-in-out infinite; animation:opacity 2s 1.25s ease-in-out infinite; }

/* First ring */
div:nth-child(2)  { left:calc(50% +  13px); }
div:nth-child(3)  { left:calc(50% -  27px); top:calc(50% +   2px); }
div:nth-child(4)  { left:calc(50% - 106px); top:calc(50% +   2px); }
div:nth-child(5)  { left:calc(50% - 145px); }
div:nth-child(6)  { left:calc(50% - 106px); top:calc(50% - 135px); }
div:nth-child(7)  { left:calc(50% -  27px); top:calc(50% - 135px); }

/* Second ring */
div:nth-child(8)  { left:calc(50% +  93px); }
div:nth-child(9)  { left:calc(50% +  53px); top:calc(50% +   2px); }
div:nth-child(10) { left:calc(50% +  13px); top:calc(50% +  70px); }
div:nth-child(11) { top:calc(50% + 70px); }
div:nth-child(12) { left:calc(50% - 145px); top:calc(50% +  70px); }
div:nth-child(13) { left:calc(50% - 185px); top:calc(50% +   2px); }
div:nth-child(14) { left:calc(50% - 225px); }
div:nth-child(15) { left:calc(50% - 185px); top:calc(50% - 135px); }
div:nth-child(16) { left:calc(50% - 145px); top:calc(50% - 204px); }
div:nth-child(17) { top:calc(50% - 204px); }
div:nth-child(18) { left:calc(50% +  13px); top:calc(50% - 204px); }
div:nth-child(19) { left:calc(50% +  53px); top:calc(50% - 135px); }

/* Third ring */
div:nth-child(20) { left:calc(50% + 171px); }
div:nth-child(21) { left:calc(50% + 133px); top:calc(50% +   2px); }
div:nth-child(22) { left:calc(50% +  93px); top:calc(50% +  70px); }
div:nth-child(23) { left:calc(50% +  53px); top:calc(50% + 138px); }
div:nth-child(24) { left:calc(50% -  27px); top:calc(50% + 138px); }
div:nth-child(25) { left:calc(50% - 106px); top:calc(50% + 138px); }
div:nth-child(26) { left:calc(50% - 185px); top:calc(50% + 138px); }
div:nth-child(27) { left:calc(50% - 224px); top:calc(50% +  70px); }
div:nth-child(28) { left:calc(50% - 264px); top:calc(50% +   2px); }
div:nth-child(29) { left:calc(50% - 304px); }
div:nth-child(30) { left:calc(50% - 264px); top:calc(50% - 135px); }
div:nth-child(31) { left:calc(50% - 224px); top:calc(50% - 204px); }
div:nth-child(32) { left:calc(50% - 184px); top:calc(50% - 272px); }
div:nth-child(33) { left:calc(50% - 106px); top:calc(50% - 272px); }
div:nth-child(34) { left:calc(50% -  27px); top:calc(50% - 272px); }
div:nth-child(35) { left:calc(50% +  53px); top:calc(50% - 272px); }
div:nth-child(36) { left:calc(50% +  93px); top:calc(50% - 204px); }
div:nth-child(37) { left:calc(50% + 133px); top:calc(50% - 135px); }

/* Fourth ring */
div:nth-child(38) { left:calc(50% + 251px); }
div:nth-child(39) { left:calc(50% + 212px); top:calc(50% +   2px); }
div:nth-child(40) { left:calc(50% + 171px); top:calc(50% +  70px); }
div:nth-child(41) { left:calc(50% + 133px); top:calc(50% + 138px); }
div:nth-child(42) { left:calc(50% +  93px); top:calc(50% + 206px); }
div:nth-child(43) { left:calc(50% +  13px); top:calc(50% + 206px); }
div:nth-child(44) { top:calc(50% + 206px); }
div:nth-child(45) { left:calc(50% - 145px); top:calc(50% + 206px); }
div:nth-child(46) { left:calc(50% - 224px); top:calc(50% + 206px); }
div:nth-child(47) { left:calc(50% - 264px); top:calc(50% + 138px); }
div:nth-child(48) { left:calc(50% - 304px); top:calc(50% +  70px); }
div:nth-child(49) { left:calc(50% - 344px); top:calc(50% +   2px); }
div:nth-child(50) { left:calc(50% - 384px); }
div:nth-child(51) { left:calc(50% - 344px); top:calc(50% - 135px); }
div:nth-child(52) { left:calc(50% - 304px); top:calc(50% - 204px); }
div:nth-child(53) { left:calc(50% - 264px); top:calc(50% - 272px); }
div:nth-child(54) { left:calc(50% - 224px); top:calc(50% - 340px); }
div:nth-child(55) { left:calc(50% - 145px); top:calc(50% - 340px); }
div:nth-child(56) { top:calc(50% - 340px); }
div:nth-child(57) { left:calc(50% +  13px); top:calc(50% - 340px); }
div:nth-child(58) { left:calc(50% +  93px); top:calc(50% - 340px); }
div:nth-child(59) { left:calc(50% + 133px); top:calc(50% - 272px); }
div:nth-child(60) { left:calc(50% + 171px); top:calc(50% - 204px); }
div:nth-child(61) { left:calc(50% + 212px); top:calc(50% - 135px); }

/* Fill in corners: first row */
div:nth-child(62) { left:calc(50% + 331px); }
div:nth-child(63) { left:calc(50% + 291px); top:calc(50% +   2px); }
div:nth-child(64) { left:calc(50% + 251px); top:calc(50% +  70px); }
div:nth-child(65) { left:calc(50% + 212px); top:calc(50% + 138px); }
div:nth-child(66) { left:calc(50% + 171px); top:calc(50% + 206px); }
div:nth-child(67) { left:calc(50% - 424px); top:calc(50% +   2px); }
div:nth-child(68) { left:calc(50% - 384px); top:calc(50% +  70px); }
div:nth-child(69) { left:calc(50% - 344px); top:calc(50% + 138px); }
div:nth-child(70) { left:calc(50% - 304px); top:calc(50% + 206px); }
div:nth-child(71) { left:calc(50% - 464px); }
div:nth-child(72) { left:calc(50% - 424px); top:calc(50% - 135px); }
div:nth-child(73) { left:calc(50% - 384px); top:calc(50% - 204px); }
div:nth-child(74) { left:calc(50% - 344px); top:calc(50% - 272px); }
div:nth-child(75) { left:calc(50% - 304px); top:calc(50% - 340px); }
div:nth-child(76) { left:calc(50% + 291px); top:calc(50% - 135px); }
div:nth-child(77) { left:calc(50% + 251px); top:calc(50% - 204px); }
div:nth-child(78) { left:calc(50% + 212px); top:calc(50% - 272px); }
div:nth-child(79) { left:calc(50% + 171px); top:calc(50% - 340px); }

@keyframes opacity {
  0%,100% { opacity:0.05; }
  50% { opacity:1; }
}
</style>