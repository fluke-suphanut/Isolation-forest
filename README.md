# Isolation Forest on NBA Players Dataset

## Overview

โปรเจกต์นี้เป็นการใช้ **Isolation Forest** สำหรับการตรวจจับค่าผิดปกติ (Anomaly Detection) ในข้อมูลนักบาสเกตบอล NBA โดยมีการนำเข้าข้อมูล ทำความสะอาด วิเคราะห์ และประเมินผล เพื่อหานักกีฬาที่มีคุณสมบัติแตกต่างจากกลุ่มตัวอย่างส่วนใหญ่

## Dataset

ใช้ข้อมูลนักบาส NBA ซึ่งประกอบด้วยคุณสมบัติต่าง ๆ เช่น ขนาดร่างกาย สถิติการเล่น และคุณลักษณะอื่น ๆ ที่เกี่ยวข้อง

## Installation

ติดตั้งไลบรารีที่จำเป็น:

   ```bash
   pip install numpy pandas matplotlib scikit-learn
   ```

## Usage

1. เปิดไฟล์ Jupyter Notebook:

   ```bash
   jupyter notebook Isolationforest.ipynb
   ```
2. รันเซลล์ตามลำดับเพื่อทำการ:

   * Import dataset
   * ตรวจสอบข้อมูล
   * ทำการแปลงและทำความสะอาดข้อมูล
   * สร้างโมเดล Isolation Forest
   * วิเคราะห์ผลลัพธ์

## Project Structure

* `Isolationforest.ipynb` — โน้ตบุ๊กหลักที่มีโค้ดและคำอธิบาย
* ส่วนต่าง ๆ ในโน้ตบุ๊ก:

  * Import dataset
  * Data preprocessing
  * Model training (Isolation Forest)
  * Visualization & Result analysis

## Results & Explanation

* โมเดล **Isolation Forest** สามารถระบุผู้เล่นที่มีคุณสมบัติแตกต่างจากผู้เล่นส่วนใหญ่ได้อย่างมีประสิทธิภาพ
* จากการวัดด้วย **ค่า RMSE** พบว่า Isolation Forest ให้ผลลัพธ์ที่ดีกว่าวิธีอื่นในการตรวจจับ Outliers สำหรับข้อมูลชุดนี้
* ผลลัพธ์แสดงออกมาในรูปกราฟและตาราง เช่น:

  * กราฟกระจาย (scatter plot) ที่แสดงผู้เล่นปกติและผู้เล่นที่ถูกตรวจจับว่าเป็น Outlier
  * ตารางที่บอกว่าผู้เล่นคนใดถูกจัดให้อยู่ในกลุ่ม Outlier
* ข้อสรุป: **Isolation Forest เป็นเทคนิคที่เหมาะสมที่สุดกับ Dataset นักบาส NBA ชุดนี้**
