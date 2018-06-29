---
title: javascript时间戳和日期字符串相互转换
date: 2018-04-28 09:23:44
categories:
- js   
---

https://www.cnblogs.com/yjf512/p/3796229.html

 	//时间戳转换
	 function getMyDate(str){ 
	     var oDate = new Date();
	     oDate.setTime(str * 1000); //str不是时间戳时不用*1000即可
	     var oYear = oDate.getFullYear(),  
	     oMonth = oDate.getMonth()+1,  
	     oDay = oDate.getDate(),  
	     oHour = oDate.getHours(),  
	     oMin = oDate.getMinutes(),  
	     oSen = oDate.getSeconds(),  
	     oTime = oYear +'-'+ getzf(oMonth) +'-'+ getzf(oDay) +' '
				+ getzf(oHour) +':'+ getzf(oMin) +':'+getzf(oSen);//最后拼接时间  
	     return oTime;  //2018-06-14 10:51:44
	 }; 
 	 //补0操作
	 function getzf(num){  
	     if(parseInt(num) < 10){  
	         num = '0'+num;  
	     }  
	     return num;  
	 }