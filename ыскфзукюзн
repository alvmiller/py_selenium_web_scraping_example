from selenium import webdriver
from selenium.webdriver.chrome.service import Service
from webdriver_manager.chrome import ChromeDriverManager
from selenium.webdriver.common.keys import Keys
from selenium.webdriver.common.by import By
from selenium.webdriver.support.ui import WebDriverWait
from selenium.webdriver.support import expected_conditions as EC

driver = webdriver.Chrome(service=Service(ChromeDriverManager().install()))

wait = WebDriverWait(driver, 10)
val = "https://alvmiller.github.io/web_page_example/"
driver.get(val)
get_url = driver.current_url
wait.until(EC.url_to_be(val))
if get_url == val:
  header=driver.find_element(By.ID, "id_SotD")
  print(header.text)
#search = driver.find_element(by=By.NAME,value="q")
#search.send_keys("Selenium")
#search.send_keys(Keys.ENTER)
