<template>
    <div id = "main">
        <form>
            <br/>
            <div>
                درخبرنامه ی ما 
                <br/>
                <b>
                    عضو شوید
                </b>
            </div>
            <br/>
            <div>
                <input type="email" placeholder="آدرس ایمیل خود را وارد کنید"/>
            </div>
            <br>
            <br>
           <div>
                <input type="submit" value="عضو شوید"/>
           </div>
        </form>
    </div>
</template>


<style scoped>
#main {
    text-align: center;
    height: 300px;
    width: 40%;
}
form{
    color: white;
    background-color: blue;
    height: inherit;
    width: auto;
}

input{
    width: 60%;
    height: 110%;
    border-radius: 10px;
}
</style>
