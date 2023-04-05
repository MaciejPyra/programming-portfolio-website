# Programming Portfolio Website

The aim of the project was to develop programming portfolio webstite to showcase the most significant personal projects in a nice form without a need to visit Github. Website is hosted directly from this GitHub repository using GitHub pages. This service converts repo files and folders into a full-fledged internet website which can be accessed via a standard URL link.

My portfolio provides examples of performed programming and data science projects. Additionally, you can find out more about my skills and technical background there. To visit the website click on my [Portfolio](https://maciejpyra.github.io/programming-portfolio-website/).


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

Hugo makes creating, managing, and maintaining a website easy. The content and presentation are separated, making it simple to change the look and feel of the site without affecting the other content. 

To build the Hugo website it is needed to create markdown files which are rendered to the HTML content during transformation process. In fact, markdown files are used to populate already prepared Hugo templates.

Github repo includes only final rendered HTML files needed to publish the website. Structure includes among others folders like:

1. about - contains index.html file building "About" page on the website
2. contact - contains index.html file building "Contact" page on the website
3. post folder - contains subfolders with project pages displayed on "Projects" page. Each subfolder has its own index.html file building specific project page
4. images - contains jpg and png images displayed on the subsequent pages of website
5. tags - contains web tags contained within the website 


<a name="desc2"></a>
### Deploying the site using GitHub Pages hosting service

GitHub Pages is GitHub feature which allows to publish website code live on the Web and make site publicly available. It is possible to specify which branch and folder to use as publishing source. The content of programming portfolio repository is deployed from the main branch. Whenever changes are pushed to the source branch, the changes in the source folder will be published to the GitHub Pages site.

Easy setup, fast publishing and HTTPS support are among the most significant strengths of GitHub Pages as the hosting service. It takes only a few simple steps to enable feature for repository and specify the source for website files. As a result, GitHub automatically publishes website and make it available at a URL based on username and repository name. Additionally, GitHub Pages offers support for HTTPS, which allows for secure connections to portfolio website. This is crucial for building the trust of the site.
