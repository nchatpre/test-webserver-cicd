# test-webserver-cicd

## ทดสอบแนวความคิด ci/cd

1. เว็บไซต์ทำงานด้วย docker โดยใช้ image nginx-latest ทำงานที่ port 3080 (http)
2. file เว็บไซต์ เก็บอยู่ที่ web-files -> /var/www/html

## การติดตั้ง

1. pull git repository
2. ใส่ file ใน directory web-files (map ไปยัง /usr/share/nginx/html ใน container)
3. รันคำสั่ง docker compose up -d
4. webserver รันที่ port 3080 ตาม docker compose file
