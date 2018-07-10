<template>        
        <footer>
            
            <div class="big">
               تمامی حقوق این سایت متعلق به دانشگاه امیر کبیر بوده و هر گونه استفاده از منابع و طراحی های این سایت توسط نهادی خارج از دانشگاه با پیگرد قانونی همرا خواهد بود
            </div>
            
            <div class="small">
                <ul>
                    اطلاعات ما
                    <li>
                        <a href="#">
                       درباره ما
                        </a>
                    </li>
                    <li>
                        <a href="#">
                       تماس با ما
                        </a>
                    </li>
                </ul>
            </div>
            
            <div class="big">
                <ul>
                    به ما در رسانه های اجتماعی بپیوندید
                    <li>
                        <SocialLogo/>
                    </li>
                    <li>
                        <SocialLogo/>
                    </li>
                </ul>
            </div>
            
            <div class="small">
                <ul>
                    خدمات مشتریان
                    <li>
                        <a href="#">
                        سوالات متداول
                        </a>
                    </li>
                    <li>
                        <a href="#">
                        بازگرداندن کالا
                        </a>
                    </li>
                    <li>
                        <a href="#">
                        شرایط استفاده
                        </a>
                    </li>
                    <li>
                        <a href="#">
                        حریم شخصی
                        </a>
                    </li>
                </ul>
            </div>
            
        </footer>
</template> 

<script >
  import SocialLogo from '@/components/SocialLogo'

  export default {
    components:{
      SocialLogo
    } 
}
</script>



<style scoped>
    footer {
         text-align: right;
         display: flex;
         background-color: gainsboro;
         height: 200px;
    }
    div.big {
      width: 30%;
      padding: 8px;
      align-self: center;
    }

    div.small {
      padding: 4px;
    }

    div{
        font-size: .7em;
        display: flex;
        height: 100%;
        margin: 0 2% 0 2%;
    }

    ul { 
         list-style-type: none;
         font-weight: bold;
         height: 100%;
         margin: 0;
         padding: 0;
    }


    a:hover{
        color: #882222;
    }

    a{
        color: #666666
    }

</style>