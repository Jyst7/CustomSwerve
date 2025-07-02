**Total Time Spent: 20 Hours**

---
title: "CustomSwerve"
author: "Jayson"
description: "My goal is to make a custom swerve drivebase with off the shelf and 3d printed parts for around $350"
created_at: "2024-05-20"
---
# June 25th: The beginning of my pain and suffering(picking a motor) 3 Hours

Today I planned to start this project properly after a couple of failed attempts to do so, there were many options to narrow down but I decided to go for a bldc motor as they are usually good for things that spin, ie. rc cars, drones and big ones are sometimes uesd for frc. So knowing that I know I also need to budget out for esc's and other electronics ideally some of the parts I will have beforehand to make it easier.

The cost of each motor should be around $20 to get a cheap enough motor that still works. After hours of reasearch and trying and failing ot find motors I finally found something that looked promising of the surpass hobby motors, usually their motors are expensive but the 3650 model seems to have a decent price on aliexpress and with the lowest kv rating I could find of 1650 which only draws 30A so I could get a cheap ESC. I was able to get the price quite low for $15 and $18 respectively, for each module I need two of these, bringing the price per module to $70 rounding for tax. A regular swerve drive has four wheels so I will design it for that but depending on price I might bring it down to three modules. This brings the total motor+esc price for this project to around $210 or $280.

<img width="791" alt="Screenshot 2025-06-25 at 11 40 12 PM" src="https://github.com/user-attachments/assets/64f5ebe3-6fb3-45d6-98dd-5a3337c48c46" />
https://www.aliexpress.com/item/1005006812605920.html?
https://www.aliexpress.com/item/1005008145047028.html?

# June 26th: Begining of modeling 4 Hours

Today I am working on the model of each swerve module, given the motors I want to get around 60-80 inches per second and to do that I only need to gear down the motor with a 2:1 ratio so i can do that with two bevel gears one on the wheel and one connecting to it then i will do some shinanigans to get it from the motor to there but otherwise all good. I found a decently large bearing that I will use from some sketchy place called Taobao

https://item.taobao.com/item.htm?abbucket=7&id=943556619196&mi_id=ArQdD1mk0Y4TTvBZydjDBpT7ul9n90ME5dFnnHbfZP7F6DHAsQhA89shsEino6iW7YP6Q8kM--DX0XeU-UcXWrqsBgmchfmlAJ4EW1dfgek&ns=1&skuId=5848268177510&utparam=%7B%22aplus_abtest%22:%2208051687b5a4403a5283bc0b785ff686%22%7D&xxc=taobaoSearch

this bearing is 80x100x10 if i remember. I hopefully will be able to 3d print most the parts if I cannot get enough accuracy I will go to a .2 nozzle instead of .4.

I saw an interesting way of making wheels for combat robotics by broken link robotics(I don't remember which video) but he custom makes wheels by having a ridgid core and then a rubber of some sort cast around it. I unfortunately am unable to do the casting but I was thinking it might be interesting to do an abs core and a petg outer part for the wheel and I'll see if that is pretty strong

<img width="390" alt="Screenshot 2025-06-26 at 9 51 09 AM" src="https://github.com/user-attachments/assets/d95dbd5c-069d-4cdf-bc1b-dc28161f4ebb" />

I spent most of today working on this part of the swerve module done. this has the bevel gears to drive the wheel as well has the starting part of the rotation of the module. I also had to make sure that everything lined up properly and that the bearing meshes, I will most likely add tolerances later but I 100% will forget some but worse things can happen.
<img width="548" alt="Screenshot 2025-06-27 at 1 59 34 PM" src="https://github.com/user-attachments/assets/a9d0b3b4-65b4-466f-a0ec-8ae6085aeac9" />

# June 27th: continueing the mechanism 8 Hours

right now I am working on the motor mounts and its slowly getting there I need to remember to add washers at some point but for now I am using 5mm hex shafts from rev which need spacers and bearings to get it to 8mm which for 10 is $30
https://www.revrobotics.com/rev-41-1528-pk20/
https://www.revrobotics.com/rev-49-1559-pk10/?searchid=0&search_query=8mm+bearing
https://www.revrobotics.com/5mm-Hex-Shafts/?searchid=4558009&search_query=hex

<img width="791" alt="Screenshot 2025-06-27 at 2 04 41 PM" src="https://github.com/user-attachments/assets/dff407c7-77f3-49de-996c-23b32cc2a9c1" />

I don't particularly want to cut my hex shafts so I plan to adjust to use the standard sizes

the current full module looks like this for the belt i am using 2gt or gt2 idk but it is 110 tooth which is 220mm i will get it from ali
https://www.aliexpress.com/item/1005004588047992.html? 

<img width="600" alt="Screenshot 2025-06-27 at 2 09 38 PM" src="https://github.com/user-attachments/assets/faae938a-9eef-4d17-ad46-996d782d09ea" />


after way too long and many hours of hitting my head against walls trying to figure out how this work the module is done, its a bit bulky and large for the size of the wheel but I'd say its a good final product

<img width="644" alt="Screenshot 2025-06-27 at 7 49 01 PM" src="https://github.com/user-attachments/assets/ef7043d2-8a6e-41ea-8788-a814671c6c7f" />

I now need to calculate the price of the whole thing for 1 module and see how many I can get. 3d printing filaments which are pla, abs, and petg are on me as I have the filaments already. bearing inserts are $10 bearings themselves are $17. the large bearing is ￥42.8 per peice or around $.30 which is a bit sus but I can only hope it arrives. hex shafts are $11.50. belt is $3. and then the big ones motors and esc is $70. this brings the total for one module up to $111.8 this means I cannot get 4 but I can get 3 for $335.4. and I can add these aluminium extrusions from rev that I have to connect them.

<img width="689" alt="Screenshot 2025-06-27 at 8 53 52 PM" src="https://github.com/user-attachments/assets/e389a17f-87a8-4511-a923-94653c718b60" />

that is the final version there is some code that I will have to write and I will connect it to a Pi Pico and a battery I have and then we have a fully custom swerve drive.

# July 1st: Making improvements 5 hours

I made some changes to the module one was a magnetic encoder that I completely forgot to add earlier, I was planning on adding more so that I could do regular position calculation on the large 2gt gear sprocket thing, while having foc on the other motor but at the moment that is not possible from what I can see. I am also making some changes so the structure is more rigid compared to the little support between each module. I also added the screws into the model. The mag encoder is aligned so whenever the magnet is on the sensor it is in the exact position needed to rotate around its centre. it doesnt look all too different in the image but there are many small changes here and there that complete it a bit more.

<img width="1089" alt="Screenshot 2025-07-02 at 2 16 13 AM" src="https://github.com/user-attachments/assets/595e2a4c-2dcd-4f88-8dc5-9379e5dfd2a0" />

I am now starting the coding section because I am procrastinating on fixing the bom. I don't really know what I am doing too much but I am planning to switch from a pi pico to a esp32 devkit of some sort prob s3 if there is a good deal so i can use bluetooth. I dont really know too much so i spent around 1 or 2 hours watching videos on the idea of how to code swerve drive and i think i am starting to get the hang of it and then I just need to put it into code. Currently deciding between python and c++ i like c++ more but idk how that will work with the esp32.

it is currently 3 am for me but I want to keep this goin so i will. most swerve drives have 4 wheels and mine has 3 i know it wont simplify the code but if I am lucky it shouldn't make it any harder than it already is going to be. finally got the bom done, was not worth the procrastination but when is it ever(I say that knowing I would do it again in a heaertbeat) i got sumerschool sleepy time then.

# July 2nd: redesign time

Welp I assumed it would come to this, i got to redesign a lot of it because the encoder is in a dumb spot and I just couldnt figure out how to do it. This saved me a lot of trouble though because of one of my friends that is a lot smarter than me but he gave me an idea based off of a design he used which is a co axial shaft for the centre so that you can still do the encoder and have the gears on that centre shaft
