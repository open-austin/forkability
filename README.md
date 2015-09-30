# forkability

Best practices for making projects easy to fork. The most important things you can do are: simplify your projects as much as possible, and

Extra Notes
https://docs.google.com/document/d/1k0k9uBXUCyIbLfwwJ4QXP5hqGNaq4UWi3SAHvjD9e_8/edit?usp=sharing

Have anything to add? Open a pull request.

- Good READMEs and deployment instructions are important.
    - Brief description of what the project does and why it exists.
    - List where all the data the app uses, where it comes from, and from how it is used. Its important to answer this question: What is the minimum amount of data do I need to get this project running?
    - List all dependencies and their versions, possibly using a tool such as Bower.
    - Make the installation section brief or put it in a separate INSTALL.md file.
    - Include screenshots or a link so people can see it in action.
- Choose a license and add it to your repo
    - Ideally just dedicate your work to the the Public Domain. The Unlicense is a good one for this.
    - Why public domain? MIT, GPL, and the rest don't answer the question of copyright.
- Don't put copyright 2015 John, Jane, Bob, etc. on every page (or even anywhere in the app).
    - As somebody forking the repo, I don't want to put your name on every page. Will you be offended that I'm removing yourname?
- Be easy to contact
    - Answer/use GitHub issues
    - Add an email to the README, or add emails to your GitHub profile
    - Specify a maintainer, and make sure the maintainer has an easy to find email
    - If your brigade or project has a Slack channel, add a link to it.
    - Simplify your app as much as possible
- Simplify your app as much as possible
    - Use simple easy to deploy technology
        - Travis CI
    - Reduce the number of dependencies
        - Do you really need mongo and memcached?
        - Do you even need a server? Can it just be static HTML + JS files hosted on GitHub Pages?
- Are you unhappy with the architecture or the code of your app? Say so in the README or an issue (and explain why). People trying to fork your app may encounter some of these same problems and have solutions. Or they may just give up.
- Keep your city specific configuration in one file
    - For example, if your app has a map with some initial coordinates, store those initial coordinates in a config file instead of making them difficult to find.



We need to do a few things to make this project easier to fork.

- [x] Format code consistently and with a popular styleguide
     - https://github.com/rdio/jsfmt
     - https://github.com/feross/standard
     - airbnb stylguide
- [ ] Convert data/*.js files to JSON
- [x] Move main html pages out of root directory
- [x] Update README with makefile instructions
  - Its important to answer this question: What is the minimum amount of data do I need to get this project running?
- [x] Move city specific config into one place
- [x] Get rid of libs from js directory and either put them into a vendor folder or include them via build tool
- [x] Move scripts into scripts directory
	- [x] park_data.rb
	- [x] download.sh
	- [x] Makefile?
- [x] Add a CONTRIBUTING.md
- [x] Specify a maintainer in the README, and make sure the maintainer has an easy to find email
- [x] List out any architecture decisions/mistakes we've made in the README
- [x] Rename the repo to austin-parks-equity



Led by Luqmaan Dawoodjee
Best practices for making projects easy to fork

-Flu Shot app - re-deploy failed!
-City took 3 months!  
Calling out the different cities - not in the Readme!

Easy to deploy apps?
-Boston GreenMap
-Chicago My Building is Recycled
-Cutepets Bot - Adoptable pets!
They inspired us -
--Mongo and Memcached - Free Azure - ReDeploy took a month.  Gave up and deployed to Heroku!
--Project didn’t need to be soo complex!
--Simplify restAPI.  Simplify Javascript.
---Break project into multiple repos
--Maybe store stuff in a google forum!
--http://sheetsu.com/

Contributing - you’re inputs will go to the public domain!

How to tie hackpads and the repo?
How do you use Github Issues?
-We rarely use the wiki
-Conversations 
-Project ideas - Push 
-Post a weekly status as an issue!
--OR use hackpads!?!?!
--Exponentially harder to get people to use 

Deploy work on Github Pages!
-Deployed projects to Github issues
-Can’t maintain projects on Github Issues?
-C-CAN?
-local-wiki?
-Wordpress?
-So many orgs can’t even get Wordpress up!
-Best documentation: - FusionTables - Derrik Edder in Chicago

