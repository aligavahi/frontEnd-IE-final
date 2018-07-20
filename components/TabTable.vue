<template>
<div class="container">
  <ul class="nav nav-tabs" style="align-items: center;padding-left: 35%;padding-right: 35%">
    <li class="active"><a  data-toggle="tab" href="#menu1">مشخصات محصول</a></li>
    <li><a data-toggle="tab" href="#menu2">نظرات کاربران</a></li>
  </ul>

<!--   <div class="tab-content">
    <div id="menu1" class="tab-pane fade">
    </div>
    <div id="menu2" class="tab-pane fade">
    </div>
  </div> -->
  <div>
    <table>
      <tr v-for="detail in theDetails" >
      <td> {{detail.value}}</td><td>{{detail.key}} </td>
      </tr>
    </table>
  </div>
</div>
</template>

<script>
export default {
  head: {
    script: [
      { src: 'https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js' },
      { src: 'https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js' }],
    link: [
        { rel: 'stylesheet', href: 'https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css' }
      ]
  },
  prps:["product_id"],
  computed: {
    theDetails(){return this.details[1]}
  },
  methods: {
  },
  components:{
  },
   data() {
    return {
      details:{
       1:[{key:"وزن",value:"1.1kg"},{key:"سال تولید",value:"2017"},{key:"گارانتی",value:"ندارد"},{key:"ضد آب",value:" نیست"}],
       2:[{key:"وزن",value:"1.1kg"},{key:"سال تولید",value:"2017"},{key:"گارانتی",value:"ندارد"},{key:"ضد آب",value:" نیست"}],
       3:[{key:"وزن",value:"1.1kg"},{key:"سال تولید",value:"2017"},{key:"گارانتی",value:"ندارد"},{key:"ضد آب",value:" نیست"}],
       4:[{key:"وزن",value:"1.1kg"},{key:"سال تولید",value:"2017"},{key:"گارانتی",value:"ندارد"},{key:"ضد آب",value:" نیست"}],
       5:[{key:"وزن",value:"1.1kg"},{key:"سال تولید",value:"2017"},{key:"گارانتی",value:"ندارد"},{key:"ضد آب",value:" نیست"}],
       6:[{key:"وزن",value:"1.1kg"},{key:"سال تولید",value:"2017"},{key:"گارانتی",value:"ندارد"},{key:"ضد آب",value:" نیست"}],
       7:[{key:"وزن",value:"1.1kg"},{key:"سال تولید",value:"2017"},{key:"گارانتی",value:"ندارد"},{key:"ضد آب",value:" نیست"}],
       8:[{key:"وزن",value:"1.1kg"},{key:"سال تولید",value:"2017"},{key:"گارانتی",value:"ندارد"},{key:"ضد آب",value:" نیست"}],
       9:[{key:"وزن",value:"1.1kg"},{key:"سال تولید",value:"2017"},{key:"گارانتی",value:"ندارد"},{key:"ضد آب",value:" نیست"}],
       10:[{key:"وزن",value:"1.1kg"},{key:"سال تولید",value:"2017"},{key:"گارانتی",value:"ندارد"},{key:"ضد آب",value:" نیست"}],
       11:[{key:"وزن",value:"1.1kg"},{key:"سال تولید",value:"2017"},{key:"گارانتی",value:"ندارد"},{key:"ضد آب",value:" نیست"}],
       12:[{key:"وزن",value:"1.1kg"},{key:"سال تولید",value:"2017"},{key:"گارانتی",value:"ندارد"},{key:"ضد آب",value:" نیست"}],
       13:[{key:"وزن",value:"1.1kg"},{key:"سال تولید",value:"2017"},{key:"گارانتی",value:"ندارد"},{key:"ضد آب",value:" نیست"}]
      }
    }
  }
}

</script>


<style scoped>
table {
    font-family: arial, sans-serif;
    border-collapse: collapse;
    width: 100%;
    align-items: center;
}

td, th {
    text-align: right;
    padding: 8px;
}

tr:nth-child(even) {
    background-color: #dddddd;
    width: 100%;
}
</style>