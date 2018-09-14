#!/home/kalter/Desktop/venv/bin/python2.7

from selenium import webdriver
import urllib2
import time

Driver = webdriver.Chrome("/home/kalter/Desktop/chromedriver")
Driver.set_page_load_timeout(30)

def step_1():
    try:
    	Driver.get("http://www.engadget.com")
    	Driver.find_element_by_xpath("/html/body/div[1]/div[2]/div[4]/div/div[2]/form[1]/div/input").click()
        return True
    except:
        return False


def step_2():
    try:
    	Driver.refresh()
        Driver.find_element_by_xpath('//*[@id="engadget-main-dl"]/div[2]/div[1]/article/a').click()
        return True
    except:
        return False



def step_3():
    try:
    	Driver.refresh()
        Driver.find_element_by_xpath('//*[@id="engadget-main-dl"]/div[2]/div[1]/article/div[2]/div/div/div/div[4]/div/div/div[1]/span/span[2]/a').click()
        return True
    except:
        return False


while True:
    if step_1():
        print('Step 1 SUCCESS')
        break
    else:
        print('Connection ERROR')
        time.sleep(1)


while True:
	if step_2():
	    	print('Step 2 SUCCESS')
	    	break
	else:
	    print('Connection ERROR')
	    time.sleep(1)


while True:
    if step_3():
        	print('Step 3 SUCCESS')
        	break
    else:
        print('Connection ERROR')
        time.sleep(1)
