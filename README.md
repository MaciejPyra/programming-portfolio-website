# Programming Portfolio Website

The aim of the project was to develop programming portfolio webstite to showcase the most significant personal projects in a nice form without a need to visit Github. Website is hosted directly from this GitHub repository using GitHub pages. This service converts repo files and folders into a full-fledged internet website which can be accessed via a standard URL link.

My portfolio provides examples of performed programming and data science projects. Additionally, you can find out more about my skills and technical background there. To visit the abovementioned website click on my [Portfolio](https://maciejpyra.github.io/programming-portfolio-website/).


# Table of Contents

  * [Introduction](#intro)
     * [What is Hugo framework?](#intro1)
     * [Technology Stack](#intro2)
  * [How the site is built and published?](#desc)
     * [Building the site](#desc1)
     * [Deploying the site using GitHub Pages hosting service](#desc2)


<a name="intro"></a>
<a name="intro1"></a>
## Introduction
### What is Hugo framework?

<p align="center">
  <img src="https://github.com/MaciejPyra/programming-portfolio-website/blob/main/GitHub_Hugo.png" />
</p>

Hugo is one of the most popular open-source static site generators. With its amazing speed and flexibility, Hugo makes building websites fun again.

Hugo as a static site generator allows to create a website with little to no code. However, it is still possible to dive into the code to make changes to its structure. Hugo uses Go templates to make use of variables and placeholders within HTML files. Static site generators allow to write content in a simple markup language - Markdown. Then, content is transformed into static HTML files. It applies any templates or styles to pages before serving them up to the user.

All the content is static and does not change once the user is viewing the page. Due to the lack of complex interactivity, there is no need to worry about constant requests to a server, database configuration or dynamic data management.


<a name="intro2"></a>
### Technology Stack
* Hugo framework,
* Markdown,
* Git,
* GitHub pages;


<a name="desc"></a>
## How the site is built and published?

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
### Deploying the site using GitHub Pages hosting service

GitHub Pages is GitHub feature which allows to publish website code live on the Web and make site publicly available. It is possible to specify which branch and folder to use as publishing source. The content of programming poftfolio repository is deployed from the main branch. Whenever changes are pushed to the source branch, the changes in the source folder will be published to the GitHub Pages site.

Easy setup, fast publishing and HTTPS support are among the most significant strengths of GitHub Pages as the hosting service. It takes only a few simple steps to enable feature for repository and specify the source for website files. As a result, GitHub automatically publishes website and make it available at a URL based on username and repository name. Additionally, GitHub Pages offers support for HTTPS, which allows for secure connections to portfolio website. This is crucial for building the trust of the site.
