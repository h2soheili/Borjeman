#  
# اسکرین های بخش ساکن به تفکیک  عکس و پارامتر های درخواستی
پارامتر های که دارای مقدار هستن  در جلوی آنها متغیر هست و دقیقا متغیر درست ارسال می شود #.# #

<br/>
<br/>
<br/>
<img src="src/image0.png" style="width:30%;"/>
# operator:"chart"<br/>
type: "unitstatus",<br/>
buildingID: buildingID,   //  شناسه ساختمانی که واحد در ان قرار دارد
<br/>unitID: ID //  شناسه واحد



------------------------------------------------------------------------------------------------------------------------------
<img src="src/image1.png" />
# operator:"chart" <br/>
 type: "unitpercent",<br/>
 buildingID: buildingID,  //  شناسه ساختمانی که واحد در ان قرار دارد
<br/> unitID: ID, // شناسه واحد  
 <br/>status: "محاسبه شده"
 
 ------------------------------------------------------------------------------------------------------------------------------
<img src="src/image2.png" />
# operator:"getcostnot"<br/>
 userID: unit.typeuser,  //   نوع مالکیت. یعنی ساکن یا 
                                    // مالک.
                                    // نام پارامتر غلط انداز است ولی در نقش
                                    // typeyser or // usertype
                                    // به کار می رود
                                    //
                                    <br/>
 buildingID: unit.buildingID,  //شناسه ساختمانی که واحد در ان قرار دارد
 <br/> unitID: unit.ID, // شناسه واحد
 ID: "",<br/>
 type:'',<br/>
 status: "پرداخت شده",<br/> 
 time1: unix1, //تاریخ اول بر حسب یونیکس
 <br/>time2: unix2 // تاریخ دوم
------------------------------------------------------------------------------------------------------------------------------
<img src="src/image3.png" />
# operator:"getcostnot"<br/>
  userID: unit.typeuser,       
                                     // نوع مالکیت. یعنی ساکن یا 
                                    // مالک.
                                    // نام پارامتر غلط انداز است ولی در نقش
                                    // typeyser or // usertype
                                    // به کار می رود
                                    //<br/>
 typeuser:unit.typeuser,     // مشابه بالا می باشد. به علت نبود داکیو منت منسجم
                            //.در این درخواست به سرور هر دو را می فرستم                                    
  <br/>buildingID: unit.buildingID,<br/>//شناسه ساختمانی که واحد در ان قرار دارد 
  unitID: unit.ID, //شناسه واحد
  <br/>type: "",<br/>
  ID: "",<br/>
  status: "پرداخت نشده",<br/>
  time1: "",<br/>
  time2: ""

------------------------------------------------------------------------------------------------------------------------------
<img src="src/image4.png" />

طی جلسه ای که برگزار شد. اقای قنبری گفتن که تمام ساکنین و مالکین بتوانند کل هزینه های ساختمان را رویت کنند
بنابراین فیلتر ای روی پارامتر ها نگذاشته شده

چیزی که باید توجه بشه اینه که تو صفحه و در آیتم های نوشته سهم شما. در حالیکه هیج پارامتری برای مشخص کردن طرف نیست که سرور گزارش رو بر اساس آن نفر بفرستد.

# operator:"getcost"<br/>
ID: "",<br/>
unitID: "",<br/>
costID: "",<br/>
buildingID: unit.buildingID,  // شناسه ساختمان که واحد در آن است
<br/>type: "هزینه",<br/>
time1:  unix1, //تاریخ اول
<br/>time2:  unix2,  // تاریخ دوم بر حسب یونیکس
<br/>status: "محاسبه شده",<br/>
typeuser:"",<br/>
chargeeffect:''<br/>
          
<img src="src/image5.png" />
# operator:"getcost"<br/>
 ID: "",<br/>
 unitID: "",<br/>
 costID: "",<br/>
 buildingID:  unit.buildingID, //شناسه ساختمانی که واحد در آن است
 <br/>type: "هزینه ثابت",<br/>
 time1:  unix1,  //تاریخ اول
 <br/>time2:  unix2,  //تاریخ دوم
 <br/>status: "محاسبه شده",<br/>
 typeuser:''<br/>


<br/>
<br/>
<br/>
<img src="src/image6.png" />
# operator:"getcostnot"<br/>
 typeuser: unit.typeuser,  //نوع واحد. ساکن یا مالک 
 <br/>userID:unit.typeuser,  // نوع واحد.   مالک یا ساکن
 <br/>buildingID: unit.buildingID,  //شناسه ساختمانی که واحد در آن است
 <br/>unitID: unit.ID,<br/> //شناسه ساختمان
 ID: "",<br/>
 status: "پرداخت نشده",<br/>
 time1: "",<br/>
 time2: "",<br/>
 type:"آنی"
