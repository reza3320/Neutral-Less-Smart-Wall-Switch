# Neutral-Less-Smart-Wall-Switch

Most buildings have "Neutral" wiring in all of their wall switches and plugs but some old or none standard buildings don't have.
For this king of buildings you need to rewire the whole unit for applying some smart swithes but with this design you don't need to.


![image](https://user-images.githubusercontent.com/72464277/201483817-3e9a5f39-d4a5-481a-904d-7334874f2a06.png)
![image](https://user-images.githubusercontent.com/72464277/201483870-30e995f5-3a12-4032-83e8-75dc9b88ce2f.png)


----------------------------------------------------------------------------------------------------------------------

For our smart switch we need a power supply, in case we don't want to use battery, we have to give our switch a neutral wire but we don't have one.
So what shall we do?

let's first compare the current flowing in our wiring while the switch is OFF and ON.
While the switch is OFF, the hot wire is like this:


![image](https://user-images.githubusercontent.com/72464277/201484007-fffb1320-c07b-4641-88cd-bb546dc82f7f.png)


But when the lamp is on, it's like this:


![image](https://user-images.githubusercontent.com/72464277/201484073-151c5d52-e017-49d7-af5b-15b26b63fbf1.png)


Now all of the wires have current and all of them are dangerous like hell!
Did you see my point of comparing this? while the lamp is off, we have one neutral wire in our switch!😈

![image](https://user-images.githubusercontent.com/72464277/201484165-3b281cd2-fe3b-4db2-88a1-65b8305dc4af.png)

How can this neutral wire can help us?
An AC to DC convertor can be made with different methods, but in our case that we just a little amount of current for our microcontroller and also we have a limitted space in our wallswith we shoud use a switched mode power supply (SMPS). what does it mean?

Let's take a look at a simple diagram of this converter.

![image](https://user-images.githubusercontent.com/72464277/201485693-4dd8a84f-f928-45dc-a608-24d772bb3ff8.png)


The rectifier convert the current from 220v Dc to 220v AC.
For converting 220v dc to 5v dc we need the transformer to operate and transformer works with alternative current(AC).
so we need to make the current alternate with and oscillator circuit that runs around 20mHz.
Now the transformer do it's job and pass the 5v dc to a rectifier and the rectifier smooth and rectify the oscillating 5v current and deliver it to us.

The complete schematic for this SMPS is this:





The frequency of AC power line is 50/60 Hz.
If you draw the voltage-time chart of an AC lin, your chart will be like this:


![image](https://user-images.githubusercontent.com/72464277/201484521-86a3cf8b-ee31-4a8e-add7-b9d1865d07c7.png)


I talk about 220v 50Hz cause this smart switch is base on it.
in the 50Hz current, voltage is 0 on 0,10,20,30, etc millisecond. so if we cut the line in those moment, we won't lose much current, but it can power our circuit for controlling the switch.







![Assembly](https://user-images.githubusercontent.com/72464277/201482602-208cbb10-9aef-4506-b64e-cf4c6dacd172.png)
![Assembly1](https://user-images.githubusercontent.com/72464277/201482628-bf35b448-d1e5-4e6d-ad8c-6a6da66b11e2.png)
![Assembly2](https://user-images.githubusercontent.com/72464277/201482629-cf0e8efe-a561-4702-bf16-ddaaba4f23f5.png)
![Assembly3](https://user-images.githubusercontent.com/72464277/201482632-4f7adc86-7d0d-49a4-b610-9ff483699ef7.png)
![image](https://user-images.githubusercontent.com/72464277/201482691-ec0e07cd-ae04-45a2-acd6-a8995f873bbd.png)
![image](https://user-images.githubusercontent.com/72464277/201482737-c56571e9-3cf1-4285-a663-fc845792fdc0.png)
![image](https://user-images.githubusercontent.com/72464277/201482742-4084bf28-5482-48bd-a1a6-d5bb367135fb.png)
![image](https://user-images.githubusercontent.com/72464277/201482748-4755da0f-1f4e-4582-aac6-eb43bbec8f10.png)
![image](https://user-images.githubusercontent.com/72464277/201482752-5f35a12d-b6db-4848-aa0b-5950f613ed10.png)
![image](https://user-images.githubusercontent.com/72464277/201482755-12c7e330-c3dc-4363-81a9-68b5945b90f3.png)
![image](https://user-images.githubusercontent.com/72464277/201482770-840c25b7-eb32-44ee-a577-2bd8f8689d83.png)
![image](https://user-images.githubusercontent.com/72464277/201482776-bfc85b38-68e8-45f7-940a-a232dfd85f33.png)
![image](https://user-images.githubusercontent.com/72464277/201482780-35717e30-75fe-4e9d-875a-9bea6e09fccc.png)
![image](https://user-images.githubusercontent.com/72464277/201482774-1b004986-1cdc-4f55-8415-37d62092e0bf.png)
![image](https://user-images.githubusercontent.com/72464277/201482838-14d92937-c9e2-42ad-998e-edf246e013d0.png)
![image](https://user-images.githubusercontent.com/72464277/201483120-dc1018d4-4033-4a22-87bf-4e54aec2174c.png)
![image](https://user-images.githubusercontent.com/72464277/201482846-d3ed61f4-ee67-4e97-9a2e-53da4a62df03.png)
![image](https://user-images.githubusercontent.com/72464277/201482912-03b00ee3-9042-4871-8595-0d454ddaeb3a.png)
![image](https://user-images.githubusercontent.com/72464277/201482919-dfd7bee1-e5fc-4369-a652-469d7513c769.png)
![image](https://user-images.githubusercontent.com/72464277/201482985-6d8df0a0-75fc-4ebb-ac73-34065dede63b.png)
![image](https://user-images.githubusercontent.com/72464277/201483206-cd6f9d1f-8a46-41a3-ba0c-e2556205a307.png)
![image](https://user-images.githubusercontent.com/72464277/201483221-69a53cd0-ecae-4b17-b069-febb4c946339.png)
![image](https://user-images.githubusercontent.com/72464277/201483062-6a2ba105-455d-433b-bd91-70aa7b680984.png)
![image](https://user-images.githubusercontent.com/72464277/201483123-e6acc0fd-3105-4101-a823-b09396c52771.png)
