# Personal Portfolio
## 1. Description
This is my personal portfolio presented as a website using Astro and TypeScript, and then deployed to Cloudflare. Its main purpose is to showcase my professional skills as well as to practice and hone them even further. I also wanted to try Astro for the first time, as it is a very interesting framework as explained in section 2.1.

You can check the website clicking [here](https://noayu-portfolio.pages.dev/). It has four main pages that I plan on updating and maintaining:
| Page | Description |
| --- | --- |
| Home | It is a simple home page that presents the 3 most relevant projects that I have worked on. Clicking on one of them leads you to the Projects page which we will explain later. |
| Timeline | This page shows a timeline of my professional life, as well as my studies or additional courses that are relevant to mention. |
| Projects | Clicking on this page allows the user to see all the projects I have worked on, all the details of each project and a link to see them in GitHub. When only the README file is visible it means that the main project is private. This project of my portfolio is the best example of this. |
| About me | Page that contains information about my life, my skills and my contact, as well as an image of myself. |

## 2. Technologies used
As mentioned before I used Astro and JavaScript for this project and then deployed it to Cloudflare, but what is the reason behind the use of these technologies? Why did it have to be them? There are many answers to these questions, so let's go through them together.

### 2.1 Astro framework
Before programming I made a design about how the website should look like and what type of project it would be. The decisions are the following:

1.  It must be a **website**. Currently there are no features that require a server, so a web application would consume way too many resources for this use case.
2. It must be **multipage**. Since the amount of content will be increasing throughout the years, having a single very long page would be very tedious to read.
3. It must be **static**. It is a simple website that does not need to be reactive, and the little reactiveness it has can be manually done using TypeScript. This ensures minimal CPU consumption.
4. It needs to be **scalable** in case in the future I want to drastically change my website or new needs appear after some years.

Coincidentally, the Astro framework fulfills all these requirements at perfection.

1. Astro is a very lightweight and small framework, and optimizes any code you write. It also compacts all the pages sent to the client to minimize space and CPU consumption. It also tries to execute in the server all that can be done in the server before the files are sent to the client.
2. Astro is meant to be used in a multipage front-end project, it would not make any sense to have a single page Astro project. This happens because creating a new page in Astro is very easy, all you need to do is create a file inside the corresponding folder called *pages*, all the routing is automatically done by Astro which is very comfortable to use and one of the main reasons why one would use Astro.
3. Astro only creates **static content**. It does not mean that it can not create dynamic content of course, but by default if the programmer does not explicitly write code to create dynamic content then Astro will not create dynamic content. This has an advantage, which is that all the content that Astro sends is super light, compacted and optimized.
4. Astro allows **integration with other frameworks**. Its goal is not to compete and replace other frameworks like Angular or React, but to be used alongside them. Astro allows the creation of different components with different frameworks, even if each component uses a different one. The integration is really good and the Astro collaborators are still improving it.

Astro is a bleeding edge framework that optimizes your website and allows integration with other frameworks enabling the programmer to be versatile, and it happens to meet all the requirements for the design of my portfolio.

If I had to say a negative treat about Astro, it would be that its community is quite small, it is not a very known framework and thus, there is not much information on the Internet in contrast with React of which there are many different projects and problems solved.

### 2.2 TypeScript (and JavaScript)
TypeScript is a very widely used language for web applications, meaning that practicing it will open many doors for my professional career. I also prefer using typed variables so TypeScript is a better choice than JavaScript for me.

### 2.3 Cloudflare
There are many reasons why I chose **Cloudflare Pages**, but the thing they all have in common is that they make my website have a higher Google rating than others, since one of the things Google takes into account when rating websites is the speed at which it loads.
- Cloudflare has **CDNs all over the world**, which makes the enrouting time very short, as the distance it needs to travel from the server to the client is really short.
- It has a very **high resistance to DDoS attacks** as well as protection against common online threats.
- On top of all of this, it also offers a free plan for static websites, making it the best option that there is currently for deploying a website like this one.