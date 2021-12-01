# chanchan.github.io
#hellow.py

  from selenium import webdriver

  import time

  import os

  doc=open('log.txt','a',encoding='utf-8')

  for i in range(1,2):

	  print("第",i,"次运行")
	  print("第",i,"次……\n",file=doc)
	  driver = webdriver.Chrome() 
	  driver.maximize_window()
	  driver.get("file:///C:/Users/jWX1074906/Desktop/web/html/Hellow.html")

	  print('Before search=====================\n',file=doc)

	  print(driver.title)
	  print(driver.current_url)
	  print(driver.get_cookie)
	  print(driver.page_source)

	  print("Title===========================",file=doc)
	  print(driver.title,file=doc)
	  print("Current_url======================",file=doc)
	  print(driver.current_url,file=doc)
	  print("Cookie========================",file=doc)
	  print(driver.get_cookie,file=doc)
	  print("page_source======================",file=doc)
	  print(driver.page_source,file=doc)

	  print('After search=====================\n',file=doc)
	  os.system("@ping 127.0.0.1 -n 2 >nul")
	  driver.quit()
	
'''
常见的Selnium命令
=====================================================================

To conclude our introduction of Selenium, we’ll show you a few typical Selenium commands.
These are probably the most commonly used commands for building tests.
结束了Selenium的介绍，我们将介绍一些典型的Selenium命令，这些命令是使用最频繁的命令。

--open
  opens a page using a URL.
  使用一个URL打开一个页面。

--click/clickAndWait
  performs a click operation, and optionally waits for a new page to load.
  执行一个单击操作，并且一般要等待一段时间让新页面被导入。

--verifyTitle/assertTitle
  verifies an expected page title.
  验证一个期望页面的标题

--verifyTextPresent
  verifies expected text is somewhere on the page.
  验证在页面中出现的期望的文本是否存在。

--verifyElementPresent
  verifies an expected UI element, as defined by its HTML tag, is present on the page.
  验证一个期望出现的UI元素，一般是HTML标记对，在一个存在的页面当中。

--verifyText
  verifies expected text and it’s corresponding HTML tag are present on the page.
  验证期望出现的文本和相对应的HTML标记对。

--verifyTable
  verifies a table’s expected contents.
  验证表格中的内容。

--waitForPageToLoad
  pauses execution until an expected new page loads. Called automatically when clickAndWait is used.
  暂停执行测试直到一个期望的页面被导入。当clickAndWait使用时，waitForPageToLoad被马上执行。

--waitForElementPresent
  pauses execution until an expected UI element, as defined by its HTML tag, is present on the page.
  暂停执行测试直到一个UI元素，出现在当前页面中。
  https://hyb1996.github.io/AutoJs-Docs/#/documentation?id=inputi-text
'''

















