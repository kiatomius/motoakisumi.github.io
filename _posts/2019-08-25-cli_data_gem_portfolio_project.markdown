---
layout: post
title:      "CLI Data Gem Portfolio Project"
date:       2019-08-25 18:32:06 +0000
permalink:  cli_data_gem_portfolio_project
---


*August 25 2019*

For my CLI Data Gem Portfolio Project, I explored ways to crete a list of properties on sale on a website called Modern House (http://themodernhouse.com). The company that runs this website, Modern House, is a real estate agency firm, based in the UK, that focuses on liaising transactions of properties that are of exceptional design standards, covering both the purchase and sale sides of the transactions for their clients. I had the opportunity to view on of their listed flats in London in April 2019, and I was amazed by the quality of the design of the apartment - ever since, I have been a big fun of the website.

Not only that I have long admired the company's listed properties, I have also found the company's website to be beautiful for its simplicity of design as well as the easy of use. The website is structured in straightforward and uniform format, which I thought would be perfect for CLI Data Gem Portfolio Project.

![](https://assets.themodernhouse.com/wp-content/uploads/2019/06/Chepstow-Road-London-W2-28-950x633.jpg)

### Application

For the Final Project, I made the following design decisions:

1. CLI application lists the list of properties that are currently on 'sale' on the website.
2. CLI application then asks if the user wishes to see more information about a particular properties that might be of interest to the user.
3. CLI applicationshows more information about a particular property upon request, and gives the option to go back to the list.
4. CLI applicationexits upon receipt of the exit instruction.

Having set the design decision, I followed various instructions and tutorials that were provided on Learn platform, and constructed the application. The application initiatives via `.rb` file in the `bin` folder, which in turn refers to `cli.rb` and other `class.rb` files in the lib folders through the `env.rb` file.

### Take Away

It was my first experience to set up the connection of these different instruction/class/env files within the working environment, and due to my initial lack of knowledge on syntax relating to directories (for example, I did not know the difference between `require` and `require relative`), there were significant difficulties at first in making the application run. Learning how different files connect to each other was one of many lessons that I took away from this project, and it allowed me to understand the usefulness of `env` file, and also the importance of separating each `class` to look after one particular purpose, instead of filling all sorts of functions into a single `class`.

Another important take-away from this project was how the files can easily explode in size, and it is vital to limit the amount of information to which the application should refer. As the application went one 'level' deeper, I included a instance method called `description` that includes a relatively long description of the property, usually amounting up to three paragraphs. In my first-layer list of properties, there were roughtly 36 properties that are currently listed for sale, and including these three paragraph description for each of the 36 properties ended up slowing down the application significantly. I then made a modification to refer to only the first 500 strings of the description, and to attach the url of the description page for references to those who wants to read more about it.

I hope to further understand this control of the volume of the information in web-development, as I can imagine the volume to increase exponentially as the level of depth increases - it is perhaps something that we will cover at the SQL lessons which I am very much looking forward to.

