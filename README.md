# Software
from selenium import webdriver
from selenium.webdriver.common.by import By
import time
driver=webdriver.Chrome()
driver.get("https://www.apple.com/in/shop/buy-iphone")
driver.maximize_window()
time.sleep(5)
# driver.execute_script("window.scrollBy(0,500);")
# time.sleep(3)

iphone_17_pro = driver.find_element(By.XPATH, "/html/body/div[2]/div[2]/div[5]/div/div/div[2]/div[1]/div/div/div[1]/div/div/div/button")
iphone_17_pro.click()
time.sleep(5)
iphone_17_pro_visit = driver.find_element(By.XPATH, "/html/body/div[3]/div/div/div/div/div[1]/div/div[2]/div/div/div/div[1]/div/div[1]/div/button[2]")
iphone_17_pro_visit.click()
time.sleep(5)
iphone_17_pro_preorder = driver.find_element(By.XPATH, "/html/body/div[3]/div/div/div/div/div[1]/div/div[2]/div/div/div/div[1]/div/div[2]/div[2]/div[1]/div[2]/div[2]/a")
iphone_17_pro_preorder.click()
time.sleep(5)
time.sleep(10)
driver.quit()
