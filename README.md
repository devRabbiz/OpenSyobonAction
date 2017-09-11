อารัมภบท .. เกมมาริโอ้แมว
==================
จุดเริ่มต้นของเรื่องราวทั้งหมดทั้งมวลนี้
มาจากเพื่อนรุ่นน้องท่านหนึ่ง
บอกว่าเกมนี้ คลายเครียดได้สุดยอด 
ผมต้องเล่น .. อึ้ม (สงสัยหน้าผมจะเครียดนะ)

สักพัก เค้าเอามาลงให้หน้าเครื่องเลย 
มาจาก http://www.mediafire.com/file/4110vjvmjyvs16u/Neko+Mario+Eng.rar
ขนาด File size: 4.63 MB
Uploaded: 2011-04-30 01:53:52
Uploaded From: Thailand
มี Folder src: main.h, main.cpp และ loadg.cpp
ก็ต้องลองเล่นดู สรุปว่าชอบครับ
เพราะจำได้ว่าเกม Mario ผมเสียตังเล่นไปเยอะ
ตั้งแต่ประมาณปีพ.ศ.2525 ที่ใต้โรงหนังดาว

เปิดดูก็พบว่าแฟ้มไม่ใหญ่ มี source code ติดมาให้ด้วย หายากนะ
เป็นภาษา C จึงเริ่มต้นค้น และอ่านไปเรื่อย ๆ
ก็พบรายละเอียดเพิ่มเติมใน github.com
ที่ https://github.com/angelXwind/OpenSyobonAction
มีแฟ้มสำคัญ คือ main.cpp, loadg.cpp, DxLib.cpp และ Makefile
ที่เห็นคือพัฒนาถึง RC2 และเป็นรุ่นที่ผม Download ออกมาทดสอบ
- Original game developer: Chiku (ちく)
- Open-source port developer: Mathew Velasquez
- Developer/maintainer of this fork: Karen／明美 (@angelXwind)

ส่วนของ README.md เค้ามีทั้งภาษาอังกฤษ และภาษาญี่ปุ่น
เกมนี้เรียกกันหลายชื่อ อาทิ Shobon no Action, Neko Mario, Cat Mario, Cat MeOUCHio
ถ้าเป็นภาษาญี่ปุ่นผมอ่านไม่ออกนะครับ

เมื่อได้สำรวจ source code แล้ว ก็ได้ไปทดลอง compile ใหม่
สรุปว่าใช้ G++ ของ MinGW และ Compile & Link ใน MSys และ CygWin
ก็กลับมาที่ github.com ของ angelXwind แล้วก็ fork 
เพื่อ upload source code และแฟ้มที่เกี่ยวข้องหลังปรับแก้เล็กน้อย

Updated:
==================
- เริ่ม fork : 6 กันยายน 2560 เพราะ compile ผ่านเมื่อเที่ยง ๆ นี่หละครับ
- อัพโหลดแฟ้ม sdl-config, lib/*, include/SDL/*, *.dll 
หลังทดสอบบน MinGW และ MinGW-w64 ที่ใช้ MSYS หากนไปวางก็จะช่วยให้ compile ง่ายขึ้น

Compile:
==================
- g++ -c main.cpp
- g++ -c loadg.cpp
- g++ -c dxlib.cpp
- g++ main.o loadg.o DxLib.o -o SyobonAction `sdl-config --libs` -lSDL_gfx -lSDL_image -lSDL_mixer -lSDL_ttf
- SyobonAction
