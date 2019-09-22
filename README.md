#  
 اسکرین های بخش ساکن به تفکیک  عکس و پارامتر های درخواستی
پارامتر های که دارای مقدار هستن  در جلوی آنها متغیر هست و دقیقا متغیر درست ارسال می شود. 


<img src="src/image0.png" />
# operator:"chart"<br/>
type: "unitstatus",<br/>
buildingID: buildingID, <br/> //  شناسه ساختمانی که واحد در ان قرار دارد
unitID: ID //  شناسه واحد



------------------------------------------------------------------------------------------------------------------------------
<img src="src/image1.png" />
# operator:"chart" <br/>
 type: "unitpercent",<br/>
 buildingID: buildingID,  <br/> //  شناسه ساختمانی که واحد در ان قرار دارد
 unitID: ID,<br/> // شناسه واحد  
 status: "محاسبه شده"
 
 ------------------------------------------------------------------------------------------------------------------------------
<img src="src/image2.png" />
# operator:"getcostnot"<br/>
 userID: unit.typeuser, <br/>//   نوع مالکیت. یعنی ساکن یا 
                                    // مالک.
                                    // نام پارامتر غلط انداز است ولی در نقش
                                    // typeyser or // usertype
                                    // به کار می رود
                                    //
                                    <br/>
 buildingID: unit.buildingID,<br/> //شناسه ساختمانی که واحد در ان قرار دارد
 unitID: unit.ID, //<br/>شناسه واحد
 ID: "",<br/>
 type:'',<br/>
 status: "پرداخت شده",<br/> 
 time1: unix1,<br/>//تاریخ اول بر حسب یونیکس
 time2: unix2 // تاریخ دوم
------------------------------------------------------------------------------------------------------------------------------
<img src="src/image3.png" />
# operator:"getcostnot"<br/>
  userID: unit.typeuser, <br/>       
                                     // نوع مالکیت. یعنی ساکن یا 
                                    // مالک.
                                    // نام پارامتر غلط انداز است ولی در نقش
                                    // typeyser or // usertype
                                    // به کار می رود
                                    //
 typeuser:unit.typeuser, <br/>   // مشابه بالا می باشد. به علت نبود داکیو منت منسجم
                            //.در این درخواست به سرور هر دو را می فرستم                                    
  buildingID: unit.buildingID,<br/>//شناسه ساختمانی که واحد در ان قرار دارد 
  unitID: unit.ID,<br/>//شناسه واحد
  type: "",<br/>
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
buildingID: unit.buildingID,<br/> // شناسه ساختمان که واحد در آن است
type: "هزینه",<br/>
time1:  unix1,<br/>//تاریخ اول
time2:  unix2, <br/>// تاریخ دوم بر حسب یونیکس
status: "محاسبه شده",<br/>
typeuser:"",<br/>
chargeeffect:''<br/>
          
<img src="src/image5.png" />
# operator:"getcost"<br/>
 ID: "",<br/>
 unitID: "",<br/>
 costID: "",<br/>
 buildingID:  unit.buildingID,<br/> //شناسه ساختمانی که واحد در آن است
 type: "هزینه ثابت",<br/>
 time1:  unix1,<br/> //تاریخ اول
 time2:  unix2,<br/> //تاریخ دوم
 status: "محاسبه شده",<br/>
 typeuser:''<br/>


<br/>
<br/>
<br/>
<img src="src/image6.png" />
# operator:"getcostnot"<br/>
 typeuser: unit.typeuser,<br/> //نوع واحد. ساکن یا مالک 
 userID:unit.typeuser,<br/> // نوع واحد.   مالک یا ساکن
 buildingID: unit.buildingID,<br/> //شناسه ساختمانی که واحد در آن است
 unitID: unit.ID,<br/> //شناسه ساختمان
 ID: "",<br/>
 status: "پرداخت نشده",
 time1: "",
 time2: "",
 type:"آنی"
