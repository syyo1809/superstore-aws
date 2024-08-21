# Superstore-Project
Dataset : [Superstore Dataset](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)<br>
&nbsp;<br>
&nbsp;<br>
Architecture
![superstoreproject drawio](https://github.com/syyo1809/superstore-aws/assets/83905993/48776c38-d959-4d47-94e4-d620676c292d)
&nbsp;<br>
&nbsp;<br>
ในบัญชี IAM สร้าง Bucket ขึ้นมาเพื่อเก็บไฟล์ข้อมูล
![createbucket](https://github.com/syyo1809/superstore-aws/assets/83905993/27f8048d-19d5-4db0-bfc6-b8b021bc6b54)
![createfolderuploadfile](https://github.com/syyo1809/superstore-aws/assets/83905993/a4ff3aa1-d1df-42ef-b95b-096a290aaf12)
&nbsp;<br>
&nbsp;<br>
ไปที่ Glue เพื่อสร้าง Database ไว้เพื่อรอเก็บข้อมูลจากการ run clawler ที่มาจาก s3 bucket
![createdbinglue](https://github.com/syyo1809/superstore-aws/assets/83905993/64745a2a-1d56-47aa-adca-adc6af8916fe)
&nbsp;<br>
&nbsp;<br>
สร้าง clawler และกำหนดสิทธื์ เพื่อเข้าถึง s3 และดึงข้อมูลจาก s3 bucket แล้วไปเก็บไว้ที่ database ที่สร้างไว้
![runclawler](https://github.com/syyo1809/superstore-aws/assets/83905993/6a29f940-b353-4759-8019-d2e76a293fa6)
&nbsp;<br>
&nbsp;<br>
หลังจากที่ run clawler แล้วก้จะได้ tables มาเพื่อรอทำการ query ใน athena ต่อไป
![tableinglue](https://github.com/syyo1809/superstore-aws/assets/83905993/8fd96923-2ddd-4cb1-86ee-7496f6e13efa)
&nbsp;<br>
&nbsp;<br>
ไปที่ athena แล้วทำการดึงข้อมูลจาก database เพื่อที่จะทำการสืบค้นข้อมูลที่ต้องการ
![querywithathena](https://github.com/syyo1809/superstore-aws/assets/83905993/2ce6b311-73ab-4316-a4a5-b5e0cac7d0c0)
&nbsp;<br>
&nbsp;<br>
และใช้ ๐uicksight เพื่อทำ dashboard
![visualization](https://github.com/syyo1809/superstore-aws/assets/83905993/9a562486-85b8-4633-89c7-0f45e339bf98)

