layout: post  
title:  "Should you use a static site generator for your next blog ?"  
author: rahul  
categories: [BLOG]  
image: assets/images/servers.jpg  
tags: [featured]  

Static site generator simply put is a tool to generate full html website without in most cases wiriting actual html, css or javascript code. You usually write your posts in a markup language like markdown and they are rendered into html by the static site generator during build time. After the **SSG** (Static Site Generator) builds your site , you will usually recieve a folder containing the html files for your website which you can upload to any webserver or web host to publish your website. 

In practice , you actually don't need to build your site or even upload the files manually because there are a lot of free services that automate all this.  For example if you are using [Jekyll](https://jekyllrb.com) (a famous Static Site Generator) and Github pages to host your website, all you need to do is to just write your posts using markdown. Github will automatically build your website and publish it whenever you add something or make any new modifications. Not just github pages , there are other services like Netlify, Cloudflare Pages , Vercel and probably many others which support static site generators. By support , I mean services that integrate easily with static site generators. Since Static Site Generators are in the end just generating html , they can be used with any webhost or webserver.  

But these services that I mentioned like [Github pages](https://pages.github.com/), [Netlify](https://www.netlify.com/) , [Vercel](https://vercel.com),[Cloudflare pages](https://pages.cloudflare.com/) etc, they automatically build and publish your website whenever you make any changes. Jekyll is one of the most popular Static Site Generators available and it is the only one supported by Github pages. But other services like Netlify support several Static Site Generators.

### Should You Use a Static Site Generator ?

The answer to the above question depends on your usecase.  For example if you are building a website that changes  a lot in realtime like a weather app or anysite that changes dynamically , then obviously a static site generator is not a good idea for that. But if you are building a portfolio or a personal website or even a company website where the content probably does not change much regularly then a static site generator is a very good option for you.

You can actually even use a Static Site Generator for your blog. Think about it, do you update all your blog posts everyday  other than adding new posts ? , Do you change the appearance/design of your blog regularly ?

No right ?

In those cases, a Static Site Generator is probably the best option for you.

Creating a dynamic full fledged cms website for your portfolio or even your blog in my opinion is a little overkill. Almost all Static Site Generators out there allows you to easily add new posts or modify old posts. You can even enable comments on your static site by using services like disqus. These are basically all the things you will ever need for a blog.

Now that we have talked about the ideal use cases for a static site generator, let's talk about the advantages of using one.

#### Advantages of Using a Static Site Generator

- Speed
  
  They are fast. Like really really fast. If you are coming from a cms, or any other dynamic site generating methods, the first thing you will notice is the speed. Since static site generators are in the end basically just generating static html for your website, the sites made using them are really fast. Because there is absolutely no processing involved,  your webserver is just serving those static files . You can even cache them easily with a CDN so as to increase the speed even further. Even the best optimized CMS powered website probably won't beat a static site interms of speed.

- Simple and in many cases free hosting
  
  If you are a beginner and your site is not yet a high traffic one , you can actually host your static site for free. I know free web hosting exists for dynamic CMS powered websites but they are really really slow services. I would never recommend you to host your Wordpress site on a free webhosting service. But since static sites doesn't require any processing , you can get away wth using free web hosting. Then there are free services like Github pages or services that have a generous free plan like Netlify or Cloudflare pages where you can host your static site for free and also get amazing performance. So simple and free webhosting is another big advantage to using Static SIte Generators.

- Security
  
  Static sites are really secure since there is no database or processing involved. So your site is basically immune from the most common attacks like sql injection attacks. 

- CDN 
  
  CDN is very easy to configure with a static website. You can serve your entire website from a CDN unlike dynamic sites where only the static assets are served from a cdn.

- Scalability
  
  A static site can scale easily especially when used with a CDN. When used with a properly configured CDN , the only requests your web server has to serve are the few requests from the CDN updating it's cache.

- Version control
  
  Most people use Static Site Generators with some version control like Git. This makes it very easy to just roll back any changes if you accidentally break your site.If you are using dynamic CMS , unless you are taking regular backups manually it might be very difficult to roll back any changes if you accidentally break your site.



Now let's look at a few disadvantages of using a static site generator

#### Disadvantages of Using a Static Site Generator

- There is a little bit of learning curve
  
  For getting most things done with a Static Site Generator, you don't need any coding knowledge. But still if you want to customize your site more, you might need some basic coding knowledge. Whereas with a CMS like WordPress, you won't even need to touch a line of code to get things done.

- Difficult to implement user management
  
  There is no native support for user management in a static site. If you want to handle user registration and login , you will probably have to use some external services.  Most sites won't require user management , so it shouldn't be a major disadvantage for you.

- No native commenting support
  
  One of the biggest disadvantages of using a static site in my opinion is the lack of out of box comments support. Don't get me wrong, it is still very easy to implement comments. You just have to use an external service like Disqus.  Infact most themes for static site generators usually comes with disqus integration built in.

- File management might get a little messy for a large site
  
  For a very large site with a ton of content, managing all those files might get a little messy. But by properly using version control like git,  this shouldn't be a major problem.

#### Most Popular Static Site Generators

- [Jekyll](https://jekyllrb.com)

- [Hugo](https://gohugo.io)

- [Pelican](https://blog.getpelican.com/)

- [Eleventy](https://www.11ty.dev/)

- [Gatsby](https://www.gatsbyjs.com/)

- [Nikola](https://getnikola.com/)

#### Conclusion

In my personal opinion , unless you are making a website that needs a lot of dynamic real time changes, you should try to use a static site generator. All the cons listed above are easily manageable for most people and the advantages you get for using a static site generator easily out weighs the disadvanatages. Because of the same reason , static site generators are immensely growing in popularity these days and more and more cms powered sites are converting to static.
