# Mahidol University QGIS Project - Salaya Campus
## แผนที่ดิจิทัลมหาวิทยาลัยมหิดล วิทยาเขตศาลายา

### ภาพรวมโครงการ
โครงการนี้เป็นการสร้างแผนที่ดิจิทัลของมหาวิทยาลัยมหิดล วิทยาเขตศาลายา โดยใช้โปรแกรม QGIS เพื่อรวบรวมและแสดงข้อมูลสถานที่สำคัญต่างๆ ภายในมหาวิทยาลัย ทำให้นักศึกษา บุคลากร และผู้มาเยือนสามารถใช้ประโยชน์ในการค้นหาสถานที่และบริการต่างๆ ได้อย่างมีประสิทธิภาพ

### เครื่องมือที่ใช้
- **QGIS** - โปรแกรมระบบสารสนเทศภูมิศาสตร์แบบโอเพนซอร์ส
- **Google Earth** - สำหรับดาวน์โหลดภาพถ่ายดาวเทียม


## รายละเอียด Layers

### 1. 🏫 Mahidol University Layer
**ประเภท:** Raster Layer
- **ที่มา:** ภาพถ่ายดาวเทียมจาก Google Earth
- **การสร้าง:** การปักหมุดและดาวน์โหลดภาพ จากนั้นสร้าง Raster Layer ใน QGIS ด้วยการอ้างอิงตำแหน่ง Latitude และ Longitude
- **วัตถุประสงค์:** เป็นพื้นฐานแผนที่หลักของมหาวิทยาลัย
  
  <img width="500" alt="Screenshot 2568-06-20 at 17 03 33" src="https://github.com/user-attachments/assets/30d98dc8-58a5-49b3-99ba-4217ff016b69" />

### 2. 🏠 Dorm Layer
**ประเภท:** Polygon
- **วัตถุประสงค์:** รวบรวมสถานที่พักอาศัยสำหรับบุคลากรและนักศึกษา
- **ประโยชน์:** ใช้เป็นแนวทางในการตัดสินใจหาที่พักอาศัย

  <img width="500" alt="Screenshot 2568-06-20 at 17 44 08" src="https://github.com/user-attachments/assets/e8562d37-15f6-4243-bb74-b04c9d4ba602" />

### 3. 🍽️ Cafeteria and Restaurant Layer
**ประเภท:** Point
- **วัตถุประสงค์:** รวบรวมตำแหน่งโรงอาหาร ร้านอาหาร และร้านขนมเครื่องดื่ม
- **ประโยชน์:** เพิ่มทางเลือกในการรับประทานอาหาร โดยเฉพาะช่วงพักกลางวัน
  
  <img width="500" alt="Screenshot 2568-06-20 at 17 45 32" src="https://github.com/user-attachments/assets/2d388ca7-7ccc-4877-8dd5-35fa92f14673" />

### 4. 🏥 Infirmary Layer
**ประเภท:** Point
- **วัตถุประสงค์:** รวบรวมสถานพยาบาลและหน่วยงานให้บริการทางการแพทย์
- **ประโยชน์:** ให้บุคลากร นักศึกษา และบุคคลภายนอกทราบตำแหน่งและประเภทการบริการ
  
  <img width="500" alt="Screenshot 2568-06-20 at 17 45 57" src="https://github.com/user-attachments/assets/35e53645-3858-4ac2-8ef6-80547af9c783" />

### 5. ⚡ AED Layer
**ประเภท:** Point
- **วัตถุประสงค์:** รวบรวมตำแหน่งจุดบริการ AED (เครื่องกระตุกหัวใจไฟฟ้าอัตโนมัติ)
- **ประโยชน์:** ช่วยให้สามารถใช้งาน AED ได้อย่างรวดเร็วในสถานการณ์ฉุกเฉิน
  
  <img width="500" alt="Screenshot 2568-06-20 at 17 46 22" src="https://github.com/user-attachments/assets/a6fa10b1-f4b3-44f1-a57a-61bd7b313e4f" />

### 6. 🎓 College Layer
**ประเภท:** Point
- **วัตถุประสงค์:** รวบรวมตำแหน่งสถานศึกษาและสถาบันวิจัย
- **ประโยชน์:** ช่วยให้ผู้สนใจทราบข้อมูลสถาบันต่างๆ สำหรับการศึกษาต่อ
  
  <img width="500" alt="Screenshot 2568-06-20 at 17 46 42" src="https://github.com/user-attachments/assets/4fcf864d-565e-4269-8046-16d597bae4d1" />

### 7. 🏧 ATM and Bank Layer
**ประเภท:** Point
- **วัตถุประสงค์:** รวบรวมตำแหน่งธนาคารและตู้ ATM
- **ประโยชน์:** อำนวยความสะดวกในการทำธุรกรรมทางการเงิน
  
  <img width="500" alt="Screenshot 2568-06-20 at 17 47 09" src="https://github.com/user-attachments/assets/bf215bce-7912-4b42-ab52-f19cb607dfbe" />

### 8. 📚 Library Layer
**ประเภท:** Polygon
- **วัตถุประสงค์:** รวบรวมตำแหน่งห้องสมุด
- **ประโยชน์:** ให้ข้อมูลตำแหน่งและเวลาเปิด-ปิดของห้องสมุด

  <img width="500" alt="Screenshot 2568-06-20 at 17 47 44" src="https://github.com/user-attachments/assets/e12a71c3-52cc-41df-a4a7-37bc17aa0e95" />
  
### 9. 📄 Photocopy Shop Layer
**ประเภท:** Point
- **วัตถุประสงค์:** รวบรวมตำแหน่งร้านถ่ายเอกสาร
- **ประโยชน์:** อำนวยความสะดวกสำหรับนักศึกษาและบุคลากร โดยเฉพาะช่วงสอบและทำโปรเจกต์

  <img width="500" alt="Screenshot 2568-06-20 at 17 48 23" src="https://github.com/user-attachments/assets/a2ccb1ec-1ead-48b1-91ff-3fc96d9c635c" />

### 10. 🚴 Bicycle Route Layer
**ประเภท:** Line
- **วัตถุประสงค์:** รวบรวมเส้นทางจักรยานภายในมหาวิทยาลัย
- **ประโยชน์:** แสดงเส้นทางต่างๆ ให้บุคลากรและนักศึกษาใช้เป็นแนวทางในการเดินทาง
  <img width="500" alt="Screenshot 2568-06-20 at 17 48 43" src="https://github.com/user-attachments/assets/079804c5-f1bc-47d3-815a-2045316bacea" />

### 11. 🏛️ Museum Layer
**ประเภท:** Polygon
- **วัตถุประสงค์:** รวบรวมตำแหน่งพิพิธภัณฑ์
- **ประโยชน์:** ให้ข้อมูลพิพิธภัณฑ์ต่างๆ สำหรับผู้สนใจเข้าเยี่ยมชม
  
  <img width="500" alt="Screenshot 2568-06-20 at 17 49 21" src="https://github.com/user-attachments/assets/e25a6e43-cb06-4afc-9008-5a896ff6b84e" />

---


