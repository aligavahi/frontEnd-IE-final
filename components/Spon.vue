<template>
  <div id="spon"> 
      <div>
        <span>تمام برند های معتبر را با ما تجربه کنید</span>
      </div>
  </div>
</template>


<style scoped>
#spon{
    background: url(/spon/spon) no-repeat center center;
    background-size: cover;
    border: 1px gray dotted;
    width: 100%;
    position: relative;
}

#spon div{
    display: table;
    width: 30%;
    height: 30px;
    position: absolute;
    left: 35%;
    top: 45%;
    color: white;
    background-color: blue;
    border-radius: 20px;
    font-size: .6em;
    padding: 0px;
    text-align: center;
}

#spon div span{
    display: table-cell;
    vertical-align: middle;
}



</style>