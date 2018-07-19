<template>
  <header>
          <div class="upper">
              <div id="search-container">
                    <form>
                        <input type="text" placeholder="Search.." name="search">
                        <button type="submit"></button>
                    </form>
              </div>
              <button style="width:auto;">ورود</button>
              <button style="width:auto;">عضویت</button>
          </div>
            
          <div class="lower">
            <ul><li>برندها</li><li>تخفیف</li> <li>ورزشی</li><li>بچگانه</li><li>زنانه</li><li>مردانه</li></ul>           
          </div>
  </header>
</template>


<style scoped>
.lower{
    align-content: center;
    border-bottom: 2px solid black;
    padding-left: 12%;
    padding-right: 12%;
    margin-bottom: 6px;
}

ul{
    padding:0px;
    list-style-type: none;
    margin-bottom: 0px;
}

ul li{
    display: inline;
    margin-left: 6%;
    margin-right: 6%;
    padding: 2px;
}

ul li:hover{
    color: blue;
    text-decoration: underline blue;
    
}

.upper{
      float: none;
      overflow: hidden;
}

#search-container {
  float: left;
}

input[type=text] {
  padding: 6px;
  margin-top: 8px;
  font-size: 17px;
  border: none;
}

#search-container button {
  float: left;
  width: 30px;
  height: 30px;
  padding: 6px 10px;
  margin-top: 8px;
  margin-right: 16px;
  background: #ddd;
  font-size: 17px;
  border: none;
  cursor: pointer;
  background-image: url(/header/search.svg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
}

@media screen and (max-width: 600px){
  input[type=text],#search-container button {
            float: none;
            display: block;
            text-align: left;
            width: 100%;
            margin: 0;
            padding: 14px;
        }

  input[type=text] {
            border: 1px solid #ccc;  
  }
}
.upper > button {
      float: right;
      border-radius: 25px;
      padding: 14px 20px;
      margin: 8px 0;
      border: none;
      cursor: pointer;
      width: 100%;
}

.upper > button:hover {
      background-color: darkgray;
}

</style>
