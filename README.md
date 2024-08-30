# AutoTest

-  สามารถสร้าง Test Case โดยที่เรา clone Gitไป เอา Folder Robot ไปเล่นก่อนได้ใช้ Vs code ส่วน seleniume จะต้องใช้ IDE ของ JAVA เช่น intelij / Eclipse 

### Robot 
- เรา Clone git folder Robot เเล้วหลังจากนั้น เราเปิด Folder ใน VScode เเละก็ กด Terminal ของ ตัว Code เพื่อ Run

![image](https://github.com/user-attachments/assets/33822479-7bd6-44f9-b201-4e135688a950)


- กด new terminal 
![image](https://github.com/user-attachments/assets/f2dfe74f-a4fc-4f3a-ad12-80712a8c9287)


- จะขึ้นหน้านี้
![image](https://github.com/user-attachments/assets/c4a0057b-d047-4087-b58f-a88085b34887)


- ให้เราพิมพ์เข้าไปในหน้าดำๆ :
 **robot .\test.robot**
    
.\ --> เข้าหา path

test.robot ชื่อไฟล์เเละนามสกุลที่มี test case


### ของ Robot AutomateTest เราสามารถเพิ่ม test ในรรดทัดนี้ได้เลย

```

***Test Cases ***
Test opening google.com using Chrome  ----> ชื่อ test
    Open Browser    ${url_google}    ${browser} ----> Action ที่ทำใน test 

Get the page title and compare
    ${title}=  Get Title
    Should Be Equal As Strings  ${title}  Google

Search using the keyword "Cheese"
    Input Text      q    Cheese
    Submit Form
    ${title}=  Get Title
    Should Be Equal As Strings  ${title}  Cheese - ค้นหาด้วย Google

test case 4 Search using the keyword "Blackpink"
..... เพิ่มได้


```
