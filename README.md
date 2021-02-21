# Web Development using the EVE API

It's great fun playing games, but what if you could use your coding skills to interact with an online game and create apps for the mobile phone, or desktop?

Well, an Application Programming Interface (API) allows you to connect two systems using code, in this case - I'm connecting a statically generated website made in Hugo - to the EVE Online Universe using an API.

EVE is a massively multiplayer online universe where you can explore, mine, bounty hunt and well all manner of spacefaring activity.

This project serves as an example of how we use web based APIs to read, write and delete data inside a game, in fact - not just games, this is how the web is built. We use one API after another to enrich our web applications to do more meaningful things.

I just want this project to be a bit of fun where you can poke and prod the EVE Online universe, just as you could say - a weather forecasting API.

Once you understand the principles for one, the general concepts are largely the same.

## This project is built using Hugo

Hugo is a static site generator written in Go. It is optimized for speed, easy use and configurability. Hugo takes a directory with content and templates and renders them into a full html website.

Hugo makes use of Markdown files with front matter for meta data.

A typical website of moderate size can be rendered in a fraction of a second. A good rule of thumb is that Hugo takes around 1 millisecond for each piece of content.

It is written to work well with any kind of website including blogs, tumbles and docs.

### This project uses a design theme called Resume-A4

Hugo can take markdown files and output HTML, instead of my spending lots of time creating how that looks design wise, you can get great professional results using a free design theme.

I've used one here to get started quicker, and professionals will often use stock designs to quickly pull together websites. What is important, is that you as a web developer understand the technologies and how they fit together.

More information on the Hugo theme, is avaliable at: https://gitlab.com/mertbakir/resume-a4

## This project is under change control in GitHub

When working with software, it's a good idea to start tracking the changes you are making to your project and there is no better way than source control for this. Unfortunately, it's a learning curve, but one you really need to get out the way.

Luckily, we have fantastic options freely avaliable today to help us solve this problem. I really recommend using GitHub, in fact - this project is already residing there. Words like clone, commit, push, pull and fancy ideas like "main" need to be part of your vocabulary. Professional pen testers use tools, these tools need code and that code quite often is held in source control systems such as git. Learn about it.

GitHub is also used by us as part of a modern engineering practice, we live in a software defined world now, its a critical skill you need - here are some steps I went through to get this project shared online.

1. Downloaded and installed git
2. Created a github account
3. Created a new SSH key on my local machine, and the public key to the github account
4. I then tested I could create a connection between my local machine and the remote github account.
5. Created an empty repository in github called learning-eve-api
6. Linked my local code repo with the remote code repo in github, using code like the following.

```bash
git init
git add -A
git commit -m 'Added my project'
git remote add origin git@github.com:[YOUR GITHUB ACCOUNT]/my-new-project.git
git push -u -f origin main
```
For a better walkthrough all the steps see this [digital ocean walkthrough.](https://www.digitalocean.com/community/tutorials/how-to-push-an-existing-project-to-github)


Anyway, that's probably enough about git and source control. You'll need to get hands on and work with it for a few days, [check out youtube](https://www.youtube.com/results?search_query=git+tutorial).

## This project uses Netlify for modern DevOps engineering

Netlify really understand what JAMStack, statically generated websites are all about and the power they give modern web developers to achieve fantastic, secure results - with less overhead and effort.

I don't want to dwell too much on JAMStack, I've done that elsewhere - for a quick recap on this architecture style of building web applications, see: https://www.netlify.com/jamstack/

We will use JAMStack to find a way to host and deploy our web site, automatically after we've "pushed" changes to our remote github code repository.

The end result - something we refer to as continuous deployment using modern web development practices that scale, are secure and are dirt cheap to host.