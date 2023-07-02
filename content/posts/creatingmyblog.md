---
title: "Creating My Blog"
date: 2023-07-02T11:45:28+02:00
draft: false
---

I've always wanted to have a blog or a personal site that could help me store/share information. It is a way a way to have the information centralized and ordered.
There are several frameworks out there that can be used for this purpose jekyll is probably one of the most popular ones. I have to say that initialy I started with jekyll but I've always wanted to learn some go and when I tried Hugo i really liked it. I seemed easy and powerfull which to me is always a good combination. Hugo has a good documentation and there are several examples out there that can help you create a blog quite fast & easy. However, most of this tutorials start from by installing themes such as Papermod which to be honest is a good point to start. In my case though I always want to learn as much as possible so isntead of using a theme I decided to go and create one myself. I have to make it clear that my site is not aiming to be perfect neither professional. It is a way to learn new things that are not realted to security and that keep my mind occupied. While I'm documenting some things, keep in mind that this is not a tutorail, indeed the tutorial that I followed was https://retrolog.io/blog/creating-a-hugo-theme-from-scratch/

So, enough talking lets begin  with some basic commands:


{{< highlight go "linenos=table,hl_lines=8,linenostart=0" >}}
    hugo new site jsayerash.github.io
    cd jsayerash.github.io
    hugo new posts/creatingmyblog.md
    hugo new theme myblog
{{< / highlight >}}

The above commands will setup almost everything that you need in order to create a very basic theme. After having completed the generated files with the content from the tutorial, you can almost run
the hugo server commad to run it locally. Now there are a couple things to notice before doing that.
In my case the file the config.toml was named hugo.toml. By default the post is created as a draft so if you do not changed the above command will not show the contents of the post. You can also run hugo server -D.

Once I was able to run the blog, I decided to start give it some color. I found this page which was nice to play with some css https://neumorphism.io/ in order to improve a little bit the buttons. 
I decided to remove the metadat. I'm not really interested on when did I published something. During my reading of the hugo documentation I find out that the following command can be used to generate a different syntax css, but for now I deciced to use the builtin.

{{< highlight go "linenos=table,hl_lines=8,linenostart=0" >}}

hugo gen chromastyles --style=monokai > syntax.css
{{< / highlight >}}

After a few hours reading the official documentation, the tutorial and talking to ChatGPT. I had something that I could be built on without much effort.