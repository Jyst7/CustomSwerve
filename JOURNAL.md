---
title: "CustomSwerve"
author: "Jayson"
description: "My goal is to make a custom swerve drivebase with off the shelf and 3d printed parts for around $350"
created_at: "2024-05-20"
---
# June 25th: The beginning of my pain and suffering(picking a motor)

Today I planned to start this project properly after a couple of failed attempts to do so, there were many options to narrow down but I decided to go for a bldc motor as they are usually good for things that spin, ie. rc cars, drones and big ones are sometimes uesd for frc. So knowing that I know I also need to budget out for esc's and other electronics ideally some of the parts I will have beforehand to make it easier.

The cost of each motor should be around $20 to get a cheap enough motor that still works. After hours of reasearch and trying and failing ot find motors I finally found something that looked promising of the surpass hobby motors, usually their motors are expensive but the 3650 model seems to have a decent price on aliexpress and with the lowest kv rating I could find of 1650 which only draws 30A so I could get a cheap ESC. I was able to get the price quite low for $15 and $18 respectively, for each module I need two of these, bringing the price per module to $70 rounding for tax. A regular swerve drive has four wheels so I will design it for that but depending on price I might bring it down to three modules. This brings the total motor+esc price for this project to around $210 or $280.

<img width="791" alt="Screenshot 2025-06-25 at 11 40 12 PM" src="https://github.com/user-attachments/assets/64f5ebe3-6fb3-45d6-98dd-5a3337c48c46" />
https://www.aliexpress.com/item/1005006812605920.html?
https://www.aliexpress.com/item/1005008145047028.html?

# June 26th: Begining of modeling

Today I am working on the model of each swerve module, given the motors I want to get around 60-80 inches per second and to do that I only need to gear down the motor with a 2:1 ratio so i can do that with two bevel gears one on the wheel and one connecting to it then i will do some shinanigans to get it from the motor to there but otherwise all good. I found a decently large bearing that I will use from some sketchy place called Taobao

https://item.taobao.com/item.htm?abbucket=7&id=943556619196&mi_id=ArQdD1mk0Y4TTvBZydjDBpT7ul9n90ME5dFnnHbfZP7F6DHAsQhA89shsEino6iW7YP6Q8kM--DX0XeU-UcXWrqsBgmchfmlAJ4EW1dfgek&ns=1&skuId=5848268177510&utparam=%7B%22aplus_abtest%22:%2208051687b5a4403a5283bc0b785ff686%22%7D&xxc=taobaoSearch

this bearing is 80x100x10 if i remember. I hopefully will be able to 3d print most the parts if I cannot get enough accuracy I will go to a .2 nozzle instead of .4.

I saw an interesting way of making wheels for combat robotics by broken link robotics(I don't remember which video) but he custom makes wheels by having a ridgid core and then a rubber of some sort cast around it. I unfortunately am unable to do the casting but I was thinking it might be interesting to do an abs core and a petg outer part for the wheel and I'll see if that is pretty strong

<img width="390" alt="Screenshot 2025-06-26 at 9 51 09 AM" src="https://github.com/user-attachments/assets/d95dbd5c-069d-4cdf-bc1b-dc28161f4ebb" />

I spent most of today working on this part of the swerve module done. this has the bevel gears to drive the wheel as well has the starting part of the rotation of the module. I also had to make sure that everything lined up properly and that the bearing meshes, I will most likely add tolerances later but I 100% will forget some but worse things can happen.
<img width="548" alt="Screenshot 2025-06-27 at 1 59 34 PM" src="https://github.com/user-attachments/assets/a9d0b3b4-65b4-466f-a0ec-8ae6085aeac9" />

# June 27th: continueing the mechanism

right now I am working on the motor mounts and its slowly getting there I need to remember to add washers at some point but for now I am using 5mm hex shafts from rev which need spacers and bearings to get it to 8mm which for 10 is $30
https://www.revrobotics.com/rev-41-1528-pk20/
https://www.revrobotics.com/rev-49-1559-pk10/?searchid=0&search_query=8mm+bearing
https://www.revrobotics.com/5mm-Hex-Shafts/?searchid=4558009&search_query=hex

<img width="791" alt="Screenshot 2025-06-27 at 2 04 41 PM" src="https://github.com/user-attachments/assets/dff407c7-77f3-49de-996c-23b32cc2a9c1" />

I don't particularly want to cut my hex shafts so I plan to adjust to use the standard sizes

the current full module looks like this for the belt i am using 2gt or gt2 idk but it is 110 tooth which is 220mm i will get it from ali
https://www.aliexpress.com/item/1005004588047992.html?

<img width="600" alt="Screenshot 2025-06-27 at 2 09 38 PM" src="https://github.com/user-attachments/assets/faae938a-9eef-4d17-ad46-996d782d09ea" />

