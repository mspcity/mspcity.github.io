---
layout: post
title:      "RUBY PGA Golf CLI Project using API"
date:       2020-06-19 22:48:18 -0400
permalink:  ruby_pga_golf_cli_project_using_api
---


I am so excited that write about this blog now.

Which means I have finished my first Project!! 

I have learned a lot from this project. and it was really good experience to apply my knowledges into program.


***- Brainstorming for topic and Choosing API***

In brainstorming for the topic of my project, I have decided something I really like. which is GOLF!


I was golf player when I was in middle school. So I picked the Golf without any hesitation.

Choosing API website was kind of challenging. Each API website has different format. and some website doesn't provide 

useful data with trial key. for the first API website I picked charge $50 for useful data.  I started with trial version. but there 

was a log of "nil" values. so I had to move to another website.  

Second one seems better, it provides useful data with trial key but there is 200 call limit per month.  I thought it is enough 

number at this time.


***- creating Ruby gem and building up the program 

command "Bundle Gem pga_golf_api". it creates basic format I need for this project.

![](https://imgur.com/fs04gRJ)

be aware that You need to use '_' underscore. not '-' dash.

because if you use '-' dash, test editor will create golf under the pga folder. 


I have added three classes inside of lib folder. which are API, CLI, Player.

and I made Enviroment.rb to manage all classed here

![](https://imgur.com/P7rzBC9h)


and I need to add some gems in gemfile 

![](https://imgur.com/eG2iFCq)

make sure command 'bundle install whenever you added some gem in gemfile.

and finally I need to add excutable file in bin folder so that I can extute later.

you will need to command 'chmod +x project-name' and check if it is excutable with command 'ls -lah'

![](https://imgur.com/eG2iFCq)


these are pretty much basic setup for my project.



***- some challenging***

first I need to bring my API in my API class 

![](https://imgur.com/F7Um8GA)

and made data into variable to use.


Player class is pretty simple. I made attributes and made initialize method. also class method .all and save method to save data.


there were some challenging stuff for CLI class. I think I speent more than half of time to build CLI class.

I can't explain every detail what happened here. but I want to point out some points that made me to spend the time most.


*- CLI menu flow*

![](https://imgur.com/AmWptZz)

it was fun to add some features to the menu. but it needs to take some times what  features should be added and
what feature will make this program more useful. 
basically this is whole idea for any programs or applications.

*- capitalization*


-  it will bring many error messages if user input is not match with the API data.

there are some example in my case.

![](https://imgur.com/xX6wV3N)

for example, "first_name"  

- it starts capital letter 'Tiger'.  but the user not always put the capital letter when they type.

so you need to use '.capitalize' to make the input case insensive.



another example, "country"

- this time, ".capitalize" didn't work for me.  it made error that i have to fix it.

country "UNITED STATES" is already written by capital letters.

but user might type capital letter or not.  

so I had to use '.upcase' to make all input to capital letter.



***-wrap up***

- I have learned a lot. and It made me to think again and again to make each method work each other.

It is not perfect at this  moment. and I really wanted to put more features but I couldn't.
(honestaly, I didn't know how to.  I need to study more for this)

but I am satisfied what I made for now. and very excited to get better for the future project.

thank you












-



















