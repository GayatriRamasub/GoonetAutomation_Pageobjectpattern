 In this Video, I have automated this website- https://www.goo-net-exchange.com/. I have automated two horizontal scroll bars. I have use the following java  
 code:

  JavascriptExecutor js = (JavascriptExecutor) d;
        
  js.executeScript("arguments[0].setAttribute('style', 'left: 1.00503%; width: 98.995%;')",price);
		
		
 js.executeScript("arguments[0].setAttribute('style', 'left: 1.00503%;')",pricespanone);
			
			
 js.executeScript("arguments[0].setAttribute('style', 'left: 100%;')",pricespantwo);
			
 js.executeScript("arguments[0].setAttribute('style', 'left: 100%;')",pricespantwo);
		
((JavascriptExecutor)d).executeScript("arguments[0].value=arguments[1]", pricetext, "¥150,000");


 JavascriptExecutor js = (JavascriptExecutor) d;
        
 js.executeScript("arguments[0].setAttribute('style', 'left: 58.1395%; width: 41.8605%;')",year);
		
 js.executeScript("arguments[0].setAttribute('style', 'left: 58.1395%;')",yearspanone);
		
 js.executeScript("arguments[0].setAttribute('style', 'left: 100%;')",yearspantwo);
		
 js.executeScript("arguments[0].setAttribute('style', 'left: 100%;')",yearspantwo);
		
 ((JavascriptExecutor)d).executeScript("arguments[0].value=arguments[1]", yeartext, "2005");

  I have used the following java code for automating dropdown. I am first making the dropdown block and then selecting the value. And then I am selecting     
  removing the additional span tag.


  Select obj=new Select(d.findElement(By.id("select_car_cd")));
		
  JavascriptExecutor executor = (JavascriptExecutor) d;
		
  executor.executeScript ("document.getElementById(\"select_car_cd\").style.display = \"block\";");
	
  executor.executeScript ("document.getElementById(\"select_car_cd\").style.visibility = \"visible\";");
	 
  Thread.sleep(2000);
    
  obj.selectByIndex(2);
    
  executor.executeScript("return document.getElementById('select_car_cd-button').remove();");

Here is a video attached for that-

https://github.com/GayatriRamasub/GoonetAutomation_Pageobjectpattern/assets/43459719/8688b031-663d-439a-a3a3-1fdb7a63a54f

 
