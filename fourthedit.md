Video Order:>>>>>>>>>>>>>>>>>>>>



*************When it comes to videoing the self; the order is: 
((((Potential Title:>>>>>>('in under __min?')>>>>>>>>>>> Uminion Tech #18 VLesson 001: A.) How to push your Code from Microsoft Code to a Github Repo using a Git (Bash) Terminal via SSH; B.) and integrating a .ymlFile from GitHub Actions with a Hostinger FTP to autodeploy/autobuild/autopatch your website in real time during a 'Git Add/Git Commit/Git Push' sequence. C.) and then Cloning a Repo from Github to our Microsoft Code via Git Remote using HTTPS to test if our system works. Presented by: StorytellingSalem for Uminion dot com's Union Tech #18; (a: Beginner-To-Intermediate-Level-Coding-Lesson). <<<<<<<<<<<<<<<)))

Chapter 1:> The Preview & Goal:>
((((((((((((DURING Preview:> Share these words, while the preview is happening in the background, of snipbits of your finished product; AND OF YOU "Getting it ready")))))))))))
	-"A.)Today we're going to take some essential code from our uminion.com's website, B.) put it on Github- C.) and then connect it (our code on GitHub) to Hostinger's FTP system- via Github Actions; D.) so when we Git Push; our newly-pushed-code- automatically updates our website again. E.) The goal of this educational video is to change this word: "submit" to "upload" and then F.) use git clone remote to change it back from "upload" to "submit" G.) using both a combination of HTTPS and SSH. 
Due to the headyness of what we're covering today, we ask you to politely click the like/subscribe/ and even share button to share to a coder friend you know. 
Union Tech #18 is a union of coders- & for that- you will be able to find copy pasteable code (and transcript) via somewhere in the description below of what was covered today. & with that; we will now begin; after briefly covering our Table of Contents:

(Don't read this outloud, just pause it for a second and then move on saying: "Pause to read; and with that; lets move on:"***move on***)
Chapter 1.) is the Preview & Goal.
Chapter 2.) is "Taking the essential code from our website out (so we can put it on GitHub- to then connect it back to our website through GitHub Actions)."
Chapter 3.) is us downloading all we need and integrating it with each other
Chapter 4.) Creating a GitHub Repo (& License Recomendation)
Chapter 5.) Creating an SSH Key and Connecting our Key to GitHub
Chapter 6.) Now that the SSH Key is connected, we push our Microsoft Code to the Github Repo via the Git (Bash) Terminal; & see if it worked:
Chapter 7.) Now lets connect our Hostinger FTP to our GitHub Actions & Test it.
Chapter 8.) Now We Clone this GitHub Repo with a completely new folder, from scratch; and see if we can Git Push our code from Microsoft Code to GitHub via Git(Bash) and see if our GitHub Actions .yml file autoUpdates our Hostinger's Website Via the Hostinger FTP system & GitHub Secrets:


Chapter 2.) "Taking the essential code from our website out"

1.) Preview while talking over on what we're going to do and then saying: "lets get started:"
	---------maybe the 'preview' is me 'preparing the uminion.com page' via sharing what the uminion.com webpage looks like; 
		-((((starting off with an empty browser, 
		-and then going to internet explorer, 
		-and then from there doing F12, console, 
		-and then going to uminion.com; so we can see a working console)))))
			-and testing it out with the audio to see it working via sharing: 
				-(while explaining this is our NationWide Radio, so you can just share a podcast/music/show/thought/anything and whatever- and then choose a time to air it; so for us we'll do:"Big Announcement Yall: Today we will be putting up our code on Github!")
			-(and while showing how that works; we also say; our main goal to see if this worked; is via seeing if our change from 'submit' to 'upload' for demonstration purposes, works) 
	-and then that way when im conducting the video; (i can 'start' with a 'do a zip file to backup everything' 
		-and then 'unzip in my d drive'
		-& then: remove the code: 
			-from the d drive's includes folder (the pictures and images in MY folder; to get it ready for integration) 
			-and remove the hostinger's code's includes, (the '.php files except db connection') 
				-and then we will revisit uminion.com and refresh the page; so the 'audio no longer works when trying to submit something.'  and console having errors. 
			-Then we remove fromm the 'd drive' everything else but the includes and themes folder; 
			-then from hostinger we remove the themes folder
				-then we revisit uminion.com and we should see an empty site; 
	-Then we say: "Alright! Now we're ready for our Demonstration!"

Chapter 3: Downloading Everything:

	-A.) how to download microsoft code
	-B.) how to download git bash and make it a default terminal in microsoft code (you click "new terminal" then you click "the plus button next to powershell" and choose 'git bash"
	-C.) Launching Git Bash as your default; and then:> -Note; if this is your first time using a git terminal; you must add these:
		- GIT CONFIG --GLOBAL USER.NAME <USERNAME> <<<<<<<<<<<<type in your username without the brackets 
			-so for me it'd be:>>>>>>>>>> GIT CONFIG --GLOBAL USER.NAME Salem 
		- GIT CONFIG --GLOBAL USER.EMAIL <EMAIL> <<<<<<<<<<<<<<<<< type in your email without the brackets 
			-so for me it'd be:>>>>>>>>>> GIT CONFIG --GLOBAL USER.EMAIL "StorytellingSalem@outlook.com" (or, which email am I doing?) 
Chapter 4: Creating a Repo & License Recomendation

	-A.) how to create a new repo (with readme; we want a readme for this demonstration; 
		-(((((Have somewhere written; instead of being said:>>>> 'readmes are where you put down the profile info of this repo and keep updating its description overtime like sharing its project overview, getting started instructions, contribution guidelines, licensing and attribution info, support and contact info, and stuff that can make your repo more exciting for new folk who start here in reading what you're repo is all about.' <<<<) 
	-B.) attach a brief image of why im choosing MIT license; according to the provided link:>>>https://choosealicense.com/licenses/ 

Chapter 5: Creating an SSH Key and Connecting it to GitHub
	-A.) go over to microsoft code and close it then open up the folder im going to be wanting to put up in github. 
		-opened up folder and terminal and did the safe thing>>>>>>>>>>>>>>>>>> git config --global --add safe.directory <<<<<<<<add a *space* after "directory" and type in the folder you going to be working in, for example, for me it'd be:> the folder called: "public_html" folder, in my "D" drive. so id type in:>>>>>>>>>>> git config --global --add safe.directory /d/public_html <<<<<<<<<<<<<<<<<if i get a "blue' light? (as in, NO ERROR?) then it worked! it doesnt tell you anything when it works. it only tells you when an error shows up.
	-B.)  generate SSH key:>>>>>>>>>>>>>>>>>>>  ssh-keygen -t rsa -b 4096 -C "storytellingsalem@outlook.com" (you might have to press enter two to three times. its okay to leave the answers empty/blank. makes everything easier to remember; for you and future programmers that come after you).
	-C.) copy ssh key VIA TYPING THIS IN:>>>>>>>>>>>>>>>> clip < ~/.ssh/id_ed25519.pub
	-D.) paste in github (now our microsoft code, is now connected, to github, with this ssh key).

Chapter 6: Now that the SSH Key is connected, we push our Microsoft Code to the Github Repo via the Git (Bash) Terminal; & see if it worked:
	-A.) go over to your GIT (bash) terminal and lets get started with 'moving into proper folder" via:>>>>>>> cd /d/public_html
	-B.) (((((((((((((Optional:>>>>>>> if youd like to remove any 'git init' thats in there already, type this in:>>>>>>>>>>>>> ) rm -rf .git ((((((((((((<<<<<<<<<<'git init' intializes git. while THIS CODE <<<< removes that 'git init' (like, if you want to 'remove and put in a new one'. not so necessary if this is your first time about to use git init. but its a helpful thing to know if you are ever restarting and want to "make sure your git init is not in here". IF THIS IS YOUR FIRST ONE? YOU DONT HAVE TO WORRY ABOUT THIS ONE! BUT IF YOU DID IT? WHATEVER! YOU DIDNT DO ANYTHING BAD BAD OR ANYTHING SO FEEL FREE MOVING ON TO NEXT STEP!)
	-C.) git init ((((((((((<<<<<<<<<<<this initializes your git (bash) terminal))))))))))))
	-D.) ((((((((((((Optional:>>>>>>>> This makes it so you can 'move' bigger files faster from git to github>>>>>>>>>>)))))))))) git config http.postBuffer 524288000 
	-E.) (((("connect your git(bash) to your github via SSH)))) >>>>>>>>>>>>>>>> git remote add origin <<<<<<<<<<<<<<<<<<after "origin" add, a space, and then copy paste the SSH from your github dot com's repo page.
	-F.) ((((((Optional but sometimes helpful/very highly reccommended (very highly reccommended for this demonstration):>>>>>>>>>>>>>> did you create a 'readme' on your github repository when you created a new github? if so; then add this code; BEFORE you push/send your code to github:>>>>>>>>>>>>) git pull origin main --allow-unrelated-histories 
		-(Maybe, do this in writing:>>>>> so it cnan pause video and watch and allow us to move on?>>>)(((((<<<<<<<<<<<<<<<<< sometimes github will NOT let you merge YOUR CODE with whatever code is on GITHUB, IF, THEY HAVE DIFFERENT HISTORIES (like, if you created your code on your code-editor/microsoftCode. and then try to pull something from github, which was created on github.....github will say: "ohhhNOOOOOO these have diff histories. we aint merging em." To get past this? you use the provided code; to tell github "its okay. let the two (github code; and whats on your local computer code) to merge anyways." 
	-G.) git add . <<<<<<<<<<<<<<<<<<<<<<<<<<< (yes, this means adding a space, after "add" and a PERIOD.) 
		-(Maybe, do this in writing:>>>>> so it cnan pause video and watch and allow us to move on?>>>) This <<<< "tells git, to 'add everything to the 'staging area'" (only stuff in the staging area, can be 'committed'. only stuff 'committed' can be sent over to github. in order to send stuff to github? you have to add first, then commit, then push. if you add a period after git add like:>>>> git add . <<<< you are telling git: 'add, everything." if you want only a certain folder? itd be like git add includes (to add the 'includes' folder. orrrrr: 'git add includes/DatabaseConnection.php' if you want to ONLY add the 'DatabaseConnection.php file')
	-H.) git commit -m "TypeInYourMessageHere" <<<<<<<<<<<<<<<<<<<<< 
		(Maybe, do this in writing:>>>>> so it cnan pause video and watch and allow us to move on?>>>)'-m' stands for 'leave a message' and anything you write in quotes; will tell folk (like yourself; and/or those who you are working with; what this 'commit, did.' so like, lets say your upgrading a game with a login/logout feature. after you 'pull or clone' the game (which means to: 'bring it from github to your local code editor/computer') to then 'upgrade the game('s code) with a login/logout feature.' then you first make the code for 'login' feature. commit it with a:>>>> git commit -m "Made Log In Feature Version 1 on DATE" <<<<<<<< and then; when you make the logout feature, and commit that; you're new git commit would have a message like:>>>>> git commit -m "Made Log Out Feature Version 1 on DATE" <<<<and that way; when you or anyone else looks at your github's contributions; the 'commit message' will tell them what that code was upgraded/modified with. "Good Commit Messages- Makes Life Easier for everyone. Build a good habit/practice of leaving good ones; no matter what, no matter where, no matter for whom. please and thank you -everyone.
	-I.) git push origin main 
		-(Maybe, do this in writing:>>>>> so it cnan pause video and watch and allow us to move on?>>>)<<<<<<<<<<<<<<Is the code that "pushes" to github('s "main" branch. [older github repos, called the "main" branch, the "master" branch; but now they're going through a name change of 'everyone! call it 'main' branch from now on!' type thing (((((((((((((((((optional:>>>>>>>>>>>> if 'git push origin main' didnt work; (cause you didnt 'git pull origin main --allow-unrelated-histories') Then try:> 'git push origin main --force' (AFTER, Homework:> "Learning the difference between 'git push origin main' AND 'git push origin main --force')
			-(And that should do it! go check via refreshing your github; but friendly reminder; to 'push' something to github; you have to first 'add it' then 'commit it' to then be able to ''push it').
	-J.) OPTIONAL:>>>> type in:>>>>>> history <<<<<< to get a log of all the buttons clicked. save this as an image or copy paste this into notepad if youd like to save the history of what was typed into the git terminal. (Or maybe you want to 'add history' into the 'readme' via doing in the terminal A: "echo "# Salem's Terminal History Of First Commit To GitHub:" >> TerminalHistoryOfInitialCommitToGitHub.md"
		-Then doing git add, git commit, and git push to see it get pushed.
	-K.) NOT RECCOMMENDED; JUST SHARING FOR YOUR OWN KNOWLEDGE:>>>>>>> "Want to remove the SSH key? NOT RECOMMENDED! its how your 'git' connects to your github. but IF FOR SOME REASON; YOU WANT TO REMOVE THE SSH KEY YOU CREATED EARLIER FROM GIT (again; you never need to do this. when would you want to do this? when you're getting practice creating ssh keys and deleting them and creating new ones. thats about it. even then; you dont really need to do this. BUT JUST IN CASE; here's the words you are looking for:>>>>>> rm ~/.ssh/id_rsa (<<<<<<<<<<<<<AND THEN:>>>>>>>) rm ~/.ssh/id_rsa.pub (((((((((((<that should do it. or find the folder that the ssh key was saved and delete it; but also good practice learning how to tell git terminal to do this). 
		-Since this video is being used for demonstration purposes; I myself; am; removing this present ssh key and deleting its existence; while also removing it from GitHub for security purposes.

Chapter 7.) Now lets connect our Hostinger FTP to our GitHub Actions:
	-A.) First, we're going to create four entries on a random notepad:
		FTP_HOST
		FTP_USERNAME
		FTP_PASSWORD
		FTP_PORT
	B.) Now, we're going to go over to hostinger, and click FTP. Then we're going to create a new FTP, and we're going to remember our password.
		-Write down your password, in your notepad, next to:
		FTP_PASSWORD _____
		-Now we're going to look at our username, and see that hostinger changed our username. we are going to copy paste our username, next to:
		FTP_USERNAME _____
		-Now we're going to scroll up to the Port, and we're going to copy paste the number of the port, next to:
		FTP_PORT ____
		-Now for the last one, we're going to look at FTP_HOST, and we're only going to take the numbers/the words; that come after: "____" (so for me, it says, ___ and I am NOT going to take that part; only the numbers part. and im going to put that in my notepad here:
		FTP_HOST
	C.) I am now, going to go back to GitHub.
		-I am going to click "settings" and then scroll down till I can click "Secrets and variables" and then click "Actions."
		-I am now going to click: "New repository secret"
			-and for the title, im going to type in:
				FTP_HOST
				-and then im going to copy paste what I wrote down in notepad next to FTP_HOST, WITHOUT, copy pasting the words: "FTP_Host" (so only the numbers, go in the 'secret')
		-I am now going to click 'add new repository secret' and do the same for username, password, and port, one at a time; till I have 4 secrets. My GitHub Actions, will be using these GitHub Secrets, to log into my Hostinger FTP System; to share my files from here on GitHub to hostinger.
	D.) I am now, going to go back to my GitHub repo's main page. and "Add File."
		-Then we're going to create a .github FORWARD SLASH workflows FORWARD SLASH AutoDeployWebsite.yml 
		-and inside of it; we're going to copy paste in this code (that you can find in the description below; which is an 'action made by SamKirkland called FTPDeploy')>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

# DON'T TOUCH THIS OR MODIFY THIS, JUST READ IT; ITS HELPFUL! -Salem ("Go find the "Main Code" if you're looking for a place to practice your coding)

# What this does:>>>> Part A.) "We have 2 folders. Folder 1 (the 'includes' folder) and Folder 2 (the 'main code' folder)."
# Part A.1) Folder 1 ('includes' folder:> ) has "the individual files that we create. our code, (the 'main code' in the 'main code folder') links to these files, to make sure our website works correctly. once you create a file? and you're ready to send it over to hostinger? then please read this area and look for "***Folder 1" to dissect and figure out how to attach your code to get sent over to hostinger aswell. Try not to mess this up; but do; try to figure out how this goes overtime. this is called a '.github/workflows/ .yml' <creation. (what does this mean? this means when 'github' 'scans your repo' if it sees a '.github/workflows' then it 'knows' its being told 'do a github action, and read the .yml file to learn what kind'. you can name what your yml file/github action is, before the period in the .yml (Example: "DeployBoy.yml" or "AutoLoadingWebsiteOnHostinger.yml" stuff like so; thats where you can name your yml and what this does))"
# Part A.2 Folder 2 ('includes 'main code folder') shouldnt really be touched. If you "Checked out Lesson 3" we share with you "How to build a website using hostinger themes." a few thing about "themes" A.) You can either:> "build your code from scratch" or "use a wordpress template to help structure you out." ID RATHER BUILD OUR OWN CODE FROM SCRATCH!" but, if you want to use 'woocommerce' (which 'gives a website e-commerce/selling-items capability') then using a theme:>>>>>>>>>>>>>>>>>> that comes with 'woocommerce,' (and then deleting/& building off the now deleted/empty theme- while keeping woocommerce-) means you have 'a safe way for you/your client to start accepting money with credit cards instantly; without worrying if your own custom code will have any integration features with woocommerce or figuring out how to connect to them' <<<<<<<<<<<<<<<<<<<<<<<<<< MEANING, WHAT I RECCOMMEND, AND WHAT YOU ARE SEEING, IS THIS:> 1.) If you use a wordpress theme (in our (uminion.com's) case: The "Astra" Theme [which COMES WITH WOOCOMMERCE PREINSTALLED AND EASY TO CONNECT TO via just adding /shop or /cart or /checkout to the end of your website's name (like uminion.com/shop uminion.com/cart uminion.com/checkout <<<THIS IS WHAT "woocommerce prepackaged in" LOOKS LIKE! you 'get the astra theme' then 'delete everything except the woocommerce part in the astra theme' and then 'build your own code on top of it')]) 2.) Now here's where it gets tricky. "because its a THEME? then when 'astra, upgrades their theme(astra)'s code? Then you lose all your stuff. darn. The way to AVOID THIS? is you look at "astra" as a "parent". and then you create a child theme from it. (in our case: "Astra-Child"). this way, when "astra"(the company; does a 'theme update') and "kicks everyone off astra" WELLLLLL!!!! YOUUUUUU WONT BE KICKED OFFFFFFF, BECAUSEEEEE "astra's code is in the parent not the child" 3.) So to make sure we have our "astra-child" HOOK, ONTO, THE "Astra parent", THEN WHEN WE LOOK AT OUR "Themes" FOLDER, WE SEE 3 FILES (The first of three being a css that we dont touch (we do css in the main code). the second of three being the main code, called front page. AND THE THIRD OF THREE FILES INSIDE OUR "Themes/astra-child" FOLDER IS:>>>>> "a custom made wordpress plugin, that tells our astra-parent, we are putting our page ('front-page')'on top of the astra-parent.'" this is called; the 'functions' page. 4.) I highly highly highly recommend (not touching but:) learning how this 'functions' page works. this is not html, css, or javascript. this is a different coding language called: "Wordpress plugin". thats the coding language. thats what it looks like. thats what it does. if and when you create a website, using a (parent)theme, to adopt woocommerce/ecommerce capability, and want YOUR website to 'lay over the main (wordpress) theme' you then: A.) create the (wordpress) child theme (astra-child) B.) create the 'Functions wordpressplugin' that will connect your 'front page/index/main landing page' to overlap over the (parents)themes page (so that way, if and when 'astra' (or whoever you choose) 'updates their theme' your stuff doesnt get kicked off. cause its in a different folder, a child of that theme to stay connected to woocommerce (and not lose track of your product during maintenance updates), and uses the functions page to help connect the child theme (in our case: "***Folder 2 contents including main code". and THIS .yml file THAT YOU SEE BELOW, IS HOW TO SEND THE 'astra-child' THEME, INTO, THE "Themes folder" WHICH HAS THE "Astra-parent" OVER IN HOSTINGER (You, do not, have access to that; cause its irrelevant to us. we just need the 'astra-child' so you can 'learn how to create a functions page and main code and the css that comes with 'this area (not really OUR css, that's inside our main code and or our 'includes folder' (Folder 1))'))).
# Part B.) TL;DR:> "This sends our two folders, over to hostinger, for autodeployment; when things get git pushed." -Salem


#>>>>>>>>>>>>>>>>>>The code below this, is the .yml file to 'autodeploy from github to hostinger using a 'github action.' -Salem (if you're gonna copy paste, and tell an ai to do 'something like this but more for yourself with diff file names and folder locations;' copy whats in between:>>>>>>>>>>>>>>>>>>> & <<<<<<<<<<<<<<<<<<<<<<<<<<<<<< (and remove my lil notes in folder 1 and 2))

name: Deploy to Hostinger via FTP

on:
  push:
    branches:
      - main    # change if you deploy from a different branch
  workflow_dispatch: {}  # lets you run manually from the Actions tab

jobs:
  deploy:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout repository
        uses: actions/checkout@v4

      # Optional: show what commit is deploying
      - name: Show git status
        run: |
          git rev-parse --short HEAD
          ls -la

      # (***Folder 1, what gets sent over with Folder 1 the 'includes' (read it and figure out how to add your own without messing it up please- thank you -Salem)) 
      # Prepare an includes-bundle directory with only the files you want to upload
      - name: Prepare includes bundle
        run: |
          set -e
          mkdir -p includes-bundle
          cp includes/AudioScheduledTimeBackUp.php includes-bundle/
          cp includes/checkAudioPlayed.php includes-bundle/
          cp includes/fetchFiles.php includes-bundle/
          cp includes/filterExpiredEntries.php includes-bundle/
          cp includes/getHistoricalArchive.php includes-bundle/
          cp includes/getPopularityArchive.php includes-bundle/
          cp includes/getRandomArchive.php includes-bundle/
          cp includes/getRecentArchive.php includes-bundle/
          cp includes/getScheduledMp3s.php includes-bundle/
          cp includes/getScheduledVideos.php includes-bundle/
          cp includes/getUpcomingVideos.php includes-bundle/
          cp includes/logout.php includes-bundle/
          cp includes/submitMp3.php includes-bundle/
          cp includes/updateAudioPlayedStatus.php includes-bundle/
          cp includes/updateAudioTimePlayed.php includes-bundle/
          cp includes/updateAudioTimes.php includes-bundle/
          cp includes/UpdateSkippedAudio.php includes-bundle/
          cp includes/updateVideoAsPlayed.php includes-bundle/
          cp includes/updateVideoPlayed.php includes-bundle/
          cp includes/updateVideoStatus.php includes-bundle/
          cp includes/uploadRecordedAudio.php includes-bundle/
          cp includes/VideoSubmit.php includes-bundle/
          cp includes/VoteDown.php includes-bundle/
          cp includes/VoteUp.php includes-bundle/
          echo "Bundle contents:" && ls -la includes-bundle

      # (***Folder 2, what gets sent over with Folder 2 the 'main code folder' (read it and figure out/learn how to copy/recreate your own when you want to send just 'one folder' to a location (like on a hostinger FTP system. ask ai to help create a 'github action .yml file that can sync with hostinger's FTP system to autodeploy our code and make em live' or something like that and you should be fine) please dont mess this part up/no need to modify it/just read and learn please- thank you -Salem)) 
      # Deploy the astra-child theme folder into wp-content/themes
      - name: Upload astra-child theme
        uses: SamKirkland/FTP-Deploy-Action@v4.3.4
        with:
          server: ${{ secrets.FTP_HOST }}
          username: ${{ secrets.FTP_USERNAME }}
          password: ${{ secrets.FTP_PASSWORD }}
          protocol: ftps
          port: ${{ secrets.FTP_PORT }}
          local-dir: ./wp-content/themes/
          server-dir: wp-content/themes/
          exclude: |
            **/.git*
            **/.DS_Store
            **/node_modules/**
          include: |
            astra-child/**

      # Deploy only the selected PHP files to includes
      - name: Upload selected PHP files to includes
        uses: SamKirkland/FTP-Deploy-Action@v4.3.4
        with:
          server: ${{ secrets.FTP_HOST }}
          username: ${{ secrets.FTP_USERNAME }}
          password: ${{ secrets.FTP_PASSWORD }}
          protocol: ftps
          port: ${{ secrets.FTP_PORT }}
          local-dir: ./includes-bundle/
          server-dir: includes/
          exclude: |
            **/.git*
            **/.DS_Store


#<<<<<<<<<<<<<<<<<<The code above this, is the .yml file to 'autodeploy from github to hostinger using a 'github action.' -Salem


	-E.) then click that green 'commit/create this'. and 'it should autodeploy now. we will 'go check if it worked' via clicking 'Actions' and if we see a greencheckmark; we did it; if we see anything else; this is an opportunity for you to troubleshoot. If you are copy pasting this code directly, you might be missing some files; so its good practice to give it to an ai first; and tell it to upgrade the code to send your desired files and folders and where to see it work for your desired location. 
	-F.) If our code worked? Awesome.
		-Lets check it via: Going to hostinger and seeing if the .php files were properly added into the includes folder.
		-&Lets check the themes folder and make sure it has our astra-child theme.
		-& This means, our website, is theoretically working properly again; so lets go back to our website with F12 on; to see if the console logs are working; and retrieving the proper info from our database again.
		-If all looks good, lets go back to GitHub, open up the front page folder and look for the submit button; and change it to an upload button; and then see if it automatically changed over in our website; to make sure out GitHub Actions are working properly. 


Chapter 8: Now We Clone this GitHub Repo with a completely new folder, from scratch; and see if we can Git Push our code from Microsoft Code to GitHub via Git(Bash) and see if our GitHub Actions .yml file autoUpdates our Hostinger's Website Via the Hostinger FTP system & GitHub Secrets:


-A.) create, 
	and open, an empty folder:
		-right click (the newly created empty folder) and say: "open with microsoft code."
			-then, inside the microsoft code, open the git (bash) terminal; and type in:>
		-git config --global --add safe.directory <<<<<<< then add a space, and type in where you are.

-B.) do:>>>> git init 

-C.) cd into that folder:>>>>

-D.) git clone _____url-of-what-you-are-cloning; this time using HTTPS_____

-E.) cd into that cloned folder; so for me it'd be cd testing016/
	-Then make it safe to work in with:>>>> git config --global --add safe.directory D:/testing/Testing016 <<<<or whatever file location you are in

-F.) Make any changes you want; to such cloned code (like for us, changing back 'Upload' to 'Submit')

-F.) Type in terminal:>>>> git diff --name-status

-G.) Git add .

-H.) git commit -m "with a message"

-I.) git push

-and then check both: "in github to make sure your changes were made" 
and: "hostinger" to make sure it all changed.
and: our website to see if submit has changed there too
and: do another audio to make sure it went through. if it did; we successfully cloned something from GitHub, pushed it, and watched it automatically update and change our website in real time.



Notes:>>>. 



End somewhere:> have yourself upload a randmo txt file like the instructions of conducting this video or just something; through git via pushing to a repo via https or something


when you want to talk about something specific, you do it in 'issues' like "Quests:> (then write down a bunch and just make it in the video APPEAR like overnight or so)"
and if you want to do something like:> "and if you want to talk about general/anything else- you do it over in 'community chats' like via ***checking out the Lessons 1-11+*** here: ***and making these appear overnight or so to*** to add in or so (atleast pinned folders or so or atleast one folder thats pinned) 



copy the .yml file from #14(?)! since its got notes!


((((((((((((((((Dont forget to test site after FTP to make sure it works. both audio files and themes should be working ))))))))))))))



Please Like & subscribe if you enjoyed this video; for it'll help get more ppl to check us out! and check out our website: uminion.com !
