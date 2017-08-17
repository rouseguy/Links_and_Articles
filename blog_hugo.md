Hugo

    $ brew install go  
    $ brew install hugo   

Goto directory where you want to store the blog

Let’s say:  

    $ cd ~/Documents/blogs  

    $ hugo new site myblog   
    $ cd myblog  


    $ hugo new blog/what-is-data-science.md 

We can check the structure by typing the command  
    $ tree  

    $ hugo server --theme=hugo_theme_robust --buildDrafts   

localhost:1313  

Set themes: 

    $ cd themes 
    $ git clone  https://github.com/Zenithar/hugo-theme-bleak.git 

    $ hugo server --theme=hugo-theme-bleak --buildDrafts  

Update config.toml

    $ hugo new about.md 
    $ hugo new posts/hello-world.md 
    $ mvim content/posts/hello-world.md 

    $ hugo  

    $ git clone https://github.com/rouseguy/rouseguy.github.io.git  

    $ cp -r public/* <username>.github.io/  
    $ cd <username>.github.io 
    $ git add --all 
    $ git commit -m 'First commit'  
    $ git push  




Configuring dns to point to github.io
https://www.namecheap.com/support/knowledgebase/article.aspx/9645/2208/how-do-i-link-my-domain-to-github-pages




