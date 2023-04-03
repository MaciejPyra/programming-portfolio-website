# programming-portfolio-website
My portfolio website provides examples of performed programming and data science projects.
To visit the abovementioned website click on my [Portfolio](https://maciejpyra.github.io/programming-portfolio-website/).


# Programming Portfolio Website

The aim of the project was to develop web scraping tool which is a software program designed specifically to extract (or ‘scrape’) relevant information from internet websites. By making a request to respective URLs my tool is able to find specific data in the HTML. What is important, my program is totally independent of any external website APIs and therefore is very flexible.

Please note that repo includes final source code and two Excels with results of analysis. Each of them provides real data concerning laptop names and their prices - attributes extracted directly from two websites, respectively from www.euro.com.pl and www.komputronik.pl.


# Table of Contents

  * [Introduction](#intro)
     * [What is Hugo framework?](#intro1)
     * [Technology Stack](#intro2)
  * [How the site is built and puslished?](#desc)
     * [Building the site](#desc1)
     * [Deploying the site using github Pages](#desc2)


<a name="intro"></a>
<a name="intro1"></a>
## Introduction
### What is Hugo framework?

<p align="center">
  <img src="https://github.com/MaciejPyra/web-scraping/blob/main/Web_Scraping.JPG" />
</p>

Hugo is one of the most popular open-source static site generators. With its amazing speed and flexibility, Hugo makes building websites fun again.

Hugo as a static site generator allows to create a website with little to no code. However, it is still possible to dive into the code to make changes to its structure. Hugo uses Go templates to make use of variables and placeholders within HTML files. Static site generators allow to write content in a simple markup language, in this case Markdown. Then, content is transformed into static HTML files. It applies any templates or styles to pages before serving them up to the user.

All the content is static and does not change once the user is viewing the page. Therefore, there is no need to worry about constant requests to a server, databases or dynamic data.


<a name="intro2"></a>
### Technology Stack
* Hugo framework,
* Markdown,
* Git,
* GitHub pages;


<a name="desc"></a>
## How the site is built and puslished?

<a name="desc1"></a>
### Building the site
The whole process could be dived into 5 steps:

1. Identify the target website
3. Collect URLs of the pages where you want to extract data from
4. Make a request to these URLs to get the HTML of the page
5. Use locators to find the data in the HTML
6. Save the data in a CSV file

Initially, tool makes HTTP requests respectively to www.euro.com.pl and www.komputronik.pl websites. The scraper loads the entire HTML code for the page in question. Then, received HTML is parsed by BeautifulSoup library and program starts automatic extraction of the interesting data from a given page. After analyzing one specific page, a link to the following one is searched for in its HTML. Thanks to that, tool is self-sufficient and program can jump between pages without user involvement. Finally, the most significant data is saved into a CSV format that is more useful to the end user.


<a name="desc2"></a>
### Deploying the site using github Pages

