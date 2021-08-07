from selenium import webdriver
import time
import os
from selenium.webdriver.common.keys import Keys
from selenium.webdriver import ActionChains
from selenium.webdriver.support.ui import WebDriverWait
from selenium.webdriver.support import expected_conditions as EC
from selenium import webdriver
from selenium.webdriver.chrome.options import Options
class akru_invest(webdriver):
    def __init__(self):
        webdriver.__init__(self)
        executable_path = "/webdrivers"
        os.environ["webdriver.chrome.driver"] = executable_path
        #-----------------------------------------------------
        self.driver.get("https://prototype.akru.co/")
        time.sleep(5)
        sign_button_click_selector='navbar-header-sticky-login'
        sign_button_click_found=self.Element_Waiter(wait_secs=20,method="id",selector=sign_button_click_selector)
        if sign_button_click_found:
            self.driver.find_element_by_id(sign_button_click_selector).click()
        else:
            print("Waited 20 Seconds For Login button to appear but could not find with selector : "+sign_button_click_selector)#Failure to find login button
            reason="Waited 20 Seconds For Login button to appear but could not find with selector : "+sign_button_click_selector
        login_magic_button_click_selector='//div[@id="navbar-select-magic"]'
        login_magic_button_click_found=self.Element_Waiter(wait_secs=50,method="xpath",selector=login_magic_button_click_selector)
        if login_magic_button_click_found:
            self.driver.find_element_by_xpath(login_magic_button_click_selector).click()
        else:
            print("Waited 50 Seconds For Login button to appear but could not find with selector : "+login_magic_button_click_selector)#Failure to find login button
            reason="Waited 50 Seconds For Login button to appear but could not find with selector : "+login_magic_button_click_selector
        login_magic_text_enter_selector='//input[@id="navbar-magic-email"]'
        login_magic_text_enter_found=self.Element_Waiter(wait_secs=50,method="xpath",selector=login_magic_text_enter_selector)
        if login_magic_text_enter_found:
            self.driver.find_element_by_xpath(login_magic_text_enter_selector).send_keys('abdulrehman2022@yopmail.com')
        else:
            print("Waited 50 Seconds For Login button to appear but could not find with selector : "+login_magic_text_enter_selector)#Failure to find login button
            reason="Waited 50 Seconds For Login button to appear but could not find with selector : "+login_magic_text_enter_selector
        login_magic_text_click_selector='//button[@id="navbar-magic-next"]'
        login_magic_text_click_found=self.Element_Waiter(wait_secs=50,method="xpath",selector=login_magic_text_click_selector)
        if login_magic_text_click_found:
            self.driver.find_element_by_xpath(login_magic_text_click_selector).click()
        else:
            print("Waited 50 Seconds For Login button to appear but could not find with selector : "+login_magic_text_click_selector)#Failure to find login button
            reason="Waited 50 Seconds For Login button to appear but could not find with selector : "+login_magic_text_click_selector
        self.driver.execute_script("window.open('http://www.yopmail.com/en/');")
        WebDriverWait(self.driver, 10).until(EC.number_of_windows_to_be(2))
        self.driver.switch_to.window(self.driver.window_handles[1])
        time.sleep(10)
        yopmail_ente_button_selector='//input[@class="sbut"]'
        yopmail_ente_button_found=self.Element_Waiter(wait_secs=50,method="xpath",selector=yopmail_ente_button_selector)
        if yopmail_ente_button_found:
           self.driver.find_element_by_xpath(yopmail_ente_button_selector).click()
        else:
            print("Waited 50 Seconds For Login button to appear but could not find with selector : "+yopmail_ente_button_selector)#Failure to find login button
            reason="Waited 50 Seconds For Login button to appear but could not find with selector : "+yopmail_ente_button_selector
        self.driver.switch_to.frame(self.driver.find_element_by_id("ifmail"))
        self.driver.get(self.driver.find_element_by_xpath('//a[@class="login-button bg"]').get_attribute('href'))
        #time.sleep(5)
        self.driver.switch_to.default_content()
        #time.sleep(5)
        childwindow =self.driver.window_handles[0]
        self.driver.switch_to.window(childwindow)
        self.driver.switch_to.window(self.driver.window_handles[0])
        time.sleep(2)
        self.driver.find_element_by_xpath('//a[@href="/listing"]').click(5)


        close_invest_property_button_selector='//button[@class="Toastify__close-button Toastify__close-button--success"]'
        close_invest_property_button_found=self.Element_Waiter(wait_secs=50,method="xpath",selector=close_invest_property_button_selector)
        if close_invest_property_button_found:
           self.driver.find_element_by_xpath(close_invest_property_button_selector).click()
        else:
            print("Waited 50 Seconds For Login button to appear but could not find with selector : "+close_invest_property_button_selector)#Failure to find login button
            reason="Waited 50 Seconds For Login button to appear but could not find with selector : "+close_invest_property_button_selector
        single_property_button_selector='//div[@class="status"]'
        single_property_button_found=self.Element_Waiter(wait_secs=50,method="xpath",selector=single_property_button_selector)
        if single_property_button_found:
           self.driver.find_element_by_xpath(single_property_button_selector).click()
        else:
            print("Waited 50 Seconds For Login button to appear but could not find with selector : "+single_property_button_selector)#Failure to find login button
            reason="Waited 50 Seconds For Login button to appear but could not find with selector : "+single_property_button_selector
        self.driver.find_element_by_tag_name('body').send_keys(Keys.PAGE_DOWN)
        time.sleep(10)
        invest_property_button_selector='singleProperty-secondary-invest'
        invest_property_button_found=self.Element_Waiter(wait_secs=50,method="id",selector=invest_property_button_selector)
        if invest_property_button_found:
           self.driver.find_element_by_id(invest_property_button_selector).click()
        else:
            print("Waited 50 Seconds For Login button to appear but could not find with selector : "+invest_property_button_selector)#Failure to find login button
            reason="Waited 50 Seconds For Login button to appear but could not find with selector : "+invest_property_button_selector
        final_invest_property_button_selector='singleProperty-modal-buyToken'
        final_invest_property_button_found=self.Element_Waiter(wait_secs=50,method="id",selector=final_invest_property_button_selector)
        if final_invest_property_button_found:
           self.driver.find_element_by_id(final_invest_property_button_selector).click()
        else:
            print("Waited 50 Seconds For Login button to appear but could not find with selector : "+final_invest_property_button_selector)#Failure to find login button
            reason="Waited 50 Seconds For Login button to appear but could not find with selector : "+final_invest_property_button_selector
        time.sleep(2
        )
    def Element_Waiter(self,wait_secs=0,method="",selector=""):
        seconds_to_wait_for_calender_appearence=wait_secs
        found=False
        while True:
            try:
                if method=="tag_name":
                    calendar=self.driver.find_element_by_tag_name(selector)
                elif method=="class_name":
                    calendar=self.driver.find_element_by_class_name(selector)
                elif method=="id":
                        calendar=self.driver.find_element_by_id(selector)
                elif method=="xpath":
                    calendar=self.driver.find_element_by_xpath(selector)
                found=True
                break
            except Exception as e:
                time.sleep(1)
                print("Waiting For Element "+selector)
                print("seconds remaining : "+str(seconds_to_wait_for_calender_appearence))
                seconds_to_wait_for_calender_appearence=seconds_to_wait_for_calender_appearence-1
                if seconds_to_wait_for_calender_appearence<=0:
                    break
                else:
                    continue
        return found
akru_invest_obj=akru_invest()
