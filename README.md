There's 3 parts to this:

Part 1:>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

1  git config --global --add safe.directory /d/public_html
   2  ssh-keygen -t rsa -b 4096 -C "storytellingsalem@outlook.com"
   3  clip < ~/.ssh/id_ed25519.pub
   4  cd /d/public_html
   5  rm -rf .git
   6  git init
   7  git config http.postBuffer 524288000
   8  git remote add origin git@github.com:CoolRoostah/Testing014.git
   9  git pull origin main --allow-unrelated-histories
   10  git add .
   11  git commit -m "TestingThatIThinkIGotIt Connecting Git to GitHub"
   12  git push origin main
   13  rm ~/.ssh/id_rsa
   14  rm ~/.ssh/id_rsa.pub
   15  history




Check 1.) create a repository on github
2.) opened up folder and terminal and did the safe thing>>>>>>>>>>>>>>>>>> git config --global --add safe.directory <<<<<<<<add a *space* after "directory" and type in the folder you going to be working in, for example, for me it'd be:> the folder called: "public_html" folder, in my "D" drive. so id type in:>>>>>>>>>>> git config --global --add safe.directory /d/public_html <<<<<<<<<<<<<<<<<if i get a "blue' light? (as in, NO ERROR?) then it worked! it doesnt tell you anything when it works. it only tells you when an error shows up.
3.) generate SSH key:>>>>>>>>>>>>>>>>>>>  ssh-keygen -t rsa -b 4096 -C "storytellingsalem@outlook.com" (you might have to press enter two to three times. its okay to leave the answers empty/blank. makes everything easier to remember; for you and future programmers that come after you).
4.) copy ssh key VIA TYPING THIS IN:>>>>>>>>>>>>>>>> clip < ~/.ssh/id_ed25519.pub
5.) paste in github
6.)go over to your GIT (bash) terminal and lets get started with 'moving into proper folder" via:>>>>>>> cd /d/public_html
7.) (((((((((((((Optional:>>>>>>> if youd like to remove any 'git init' thats in there already, type this in:>>>>>>>>>>>>> ) rm -rf .git ((((((((((((<<<<<<<<<<'git init' intializes git. while THIS CODE <<<< removes that 'git init' (like, if you want to 'remove and put in a new one'. not so necessary if this is your first time about to use git init. but its a helpful thing to know if you are ever restarting and want to "make sure your git init is not in here". IF THIS IS YOUR FIRST ONE? YOU DONT HAVE TO WORRY ABOUT THIS ONE! BUT IF YOU DID IT? WHATEVER! YOU DIDNT DO ANYTHING BAD BAD OR ANYTHING SO FEEL FREE MOVING ON TO NEXT STEP!)
8.) git init ((((((((((<<<<<<<<<<<this initializes your git (bash) terminal))))))))))))
9.) ((((((((((((Optional:>>>>>>>> This makes it so you can 'move' bigger files faster from git to github>>>>>>>>>>)))))))))) git config http.postBuffer 524288000 
10.) (((("connect your git(bash) to your github via SSH)))) >>>>>>>>>>>>>>>> git remote add origin git@github.com:CoolRoostah/Testing013.git
11.) ((((((Optional but sometimes helpful:>>>>>>>>>>>>>> did you create a 'readme' on your github repository when you created a new github? if so; then add this code; BEFORE you push/send your code to github:>>>>>>>>>>>>) git pull origin main --allow-unrelated-histories (((((<<<<<<<<<<<<<<<<< sometimes github will NOT let you merge YOUR CODE with whatever code is on GITHUB, IF, THEY HAVE DIFFERENT HISTORIES (like, if you created your code on your code-editor/microsoftCode. and then try to pull something from github, which was created on github.....github will say: "ohhhNOOOOOO these have diff histories. we aint merging em." To get past this? you use the provided code; to tell github "its okay. let the two (github code; and whats on your local computer code) to merge anyways." 
12.) git add . <<<<<<<<<<<<<<<<<<<<<<<<<<<this "tells git, to 'add everything to the 'staging area'" (only stuff in the staging area, can be 'committed'. only stuff 'committed' can be sent over to github. in order to send stuff to github? you have to add first, then commit, then push. if you add a period after git add like:>>>> git add . <<<< you are telling git: 'add, everything." if you want only a certain folder? itd be like git add includes (to add the 'includes' folder. orrrrr: 'git add includes/DatabaseConnection.php' if you want to ONLY add the 'DatabaseConnection.php file')
13.) git commit -m "TypeInYourMessageHere" <<<<<<<<<<<<<<<<<<<<< '-m' stands for 'leave a message' and anything you write in quotes; will tell folk (like yourself; and/or those who you are working with; what this 'commit, did.' so like, lets say your upgrading a game with a login/logout feature. after you 'pull or clone' the game (which means to: 'bring it from github to your local code editor/computer') to then 'upgrade the game('s code) with a login/logout feature.' then you first make the code for 'login' feature. commit it with a:>>>> git commit -m "Made Log In Feature Version 1 on DATE" <<<<<<<< and then; when you make the logout feature, and commit that; you're new git commit would have a message like:>>>>> git commit -m "Made Log Out Feature Version 1 on DATE" <<<<and that way; when you or anyone else looks at your github's contributions; the 'commit message' will tell them what that code was upgraded/modified with. "Good Commit Messages- Makes Life Easier for everyone. Build a good habit/practice of leaving good ones; no matter what, no matter where, no matter for whom. please and thank you -everyone.
14.) git push origin main <<<<<<<<<<<<<<Is the code that "pushes" to github('s "main" branch. [older github repos, called the "main" branch, the "master" branch; but now they're going through a name change of 'everyone! call it 'main' branch from now on!' type thing (((((((((((((((((optional:>>>>>>>>>>>> if 'git push origin main' didnt work; (cause you didnt 'git pull origin main --allow-unrelated-histories') Then try:> 'git push origin main --force' (AFTER, Homework:> "Learning the difference between 'git push origin main' AND 'git push origin main --force')
15.) NOT RECCOMMENDED; JUST SHARING FOR YOUR OWN KNOWLEDGE:>>>>>>> "Want to remove the SSH key? NOT RECOMMENDED! its how your 'git' connects to your github. but IF FOR SOME REASON; YOU WANT TO REMOVE THE SSH KEY YOU CREATED EARLIER FROM GIT (again; you never need to do this. when would you want to do this? when you're getting practice creating ssh keys and deleting them and creating new ones. thats about it. even then; you dont really need to do this. BUT JUST IN CASE; here's the words you are looking for:>>>>>> rm ~/.ssh/id_rsa (<<<<<<<<<<<<<AND THEN:>>>>>>>) rm ~/.ssh/id_rsa.pub (((((((((((<that should do it. or find the folder that the ssh key was saved and delete it; but also good practice learning how to tell git terminal to do this).
16.) OPTIONAL:>>>> type in:>>>>>> history <<<<<< to get a log of all the buttons clicked. save this as an image or copy paste this into notepad if youd like to save the history of what was typed into the git terminal. 
17.) 















****************************************************************************
For when it comes to what i wanna do/what im trying to do with this video thang. its then:>

A.) Turn on video and introduce self and what we're going to do. (maybe do this at the end so you can clip forward clips from video at intro to show during preview?)

B.) show users where to download microsoft code
C.) show users where to download git (bash) (and how to turn it into your default terminal)
D.) show users how to create new repo (and which license to choose)


E.) open folder in microsoft code
F.) start with:
	git config --global --add safe.directory /d/public_html
		((((((((((((((( add a *space* after "directory" and type in the folder you going to be working in, for example, for me it'd be:> the folder called: "public_html" folder, in my "D" drive. so id type in:>>>>>>>>>>> git config --global --add safe.directory /d/public_html <<<<<<<<<<<<<<<<<if i get a "blue' light? (as in, NO ERROR?) then it worked! it doesnt tell you anything when it works. it only tells you when an error shows up.))))))))))))))

G.) Then start creating SSH Key via:
	ssh-keygen -t rsa -b 4096 -C "storytellingsalem@outlook.com"
		((((((((((you might have to press enter two to three times. its okay to leave the answers empty/blank. makes everything easier to remember; for you and future programmers that come after you).))))))))))
		
H.) Then the way we 'copy paste' this ssh key, is via first, typing this into git:>>>
	clip < ~/.ssh/id_ed25519.pub
I.) and that "should have 'copied our SSH key, so now we're going to go to github settings to 'paste' the ssh key into github. (now our microsoft code, is now connected, to github, with this ssh key).

J.) now we're going back to our code, and we're going to start the transfer process from our microsoft code, to github, using our ssh key. the way we do that is via: going back to our code; and typing in:"
	cd /d/public_html
(((((((((to make sure we're on the same page))))))))

K.) (optional) then do: 
	rm -rf .git

L.) then do:
	git init

M.) (optional) then do: 
	git config http.postBuffer 524288000

N.) NOWWWW that our microsoft code is ready, we can connect it to our github repo via ssh like so:
	git remote add origin git@github.com:CoolRoostah/Testing014.git

O.) once connected; we're going to "pull whats on the github repo; over to us in microsoft code; like so:"
	git pull origin main --allow-unrelated-histories
((((This should allow us to see the readme file that we created in the github repo)))


P.) now we 'add' the files we have- to the 'staging area' via:
	git add .

Q.) then we 'save' whats on the 'staging area' via 'committing to it' like so:>
	git commit -m "TestingThatIThinkIGotIt Connecting Git to GitHub"

R.) Then we 'push' our code from our microsoft code, over to github, via git(bash) using this line of code:
	git push origin main
(And that should do it! go check via refreshing your github; but friendly reminder; to 'push' something to github; you have to first 'add it' then 'commit it' to then be able to ''push it').

S.) type in history in git so you can see what was clicked and done to help you get here; and maybe in the future; know what you've done differently to not get here.

T.) Please Like & subscribe if you enjoyed this video; for it'll help get more ppl to check us out! and check out our website: uminion.com !



*************When it comes to videoing the self; the order is: 
((((Potential Title: How to push Code from Microsoft code to Github using Git via SSH)))

1.) preview while talking over on what we're going to do and then saying: "lets get started:"

2.) how to download microsoft code
3.) how to download git bash and make it a default terminal in microsoft code
	-Note; if this is your first time using a git terminal; you must add these:
		- GIT CONFIG --GLOBAL USER.NAME <USERNAME> <<<<<<<<<<<<type in your username without the brackets so for me it'd be:>>>>>>>>>> GIT CONFIG --GLOBAL USER.NAME Salem 
		- GIT CONFIG --GLOBAL USER.EMAIL <EMAIL> <<<<<<<<<<<<<<<<< type in your email without the brackets so for me it'd be:>>>>>>>>>> GIT CONFIG --GLOBAL USER.EMAIL "StorytellingSalem@outlook.com"

4.) how to create a new repo

5.) go over to microsoft code and stay there till we create new ssh key & copy it
6.) go over to github and paste ssh key

7.) Now that we've setup our code editor, git bash terminal, and github repo; we're going back to microsoft code again; to: connect our code to github till its done. 



<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<

Part 2:>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>



((((((Extra?:>>>> check out name: https://youtu.be/BIKhDVoEuvE?si=TnOgf9dMinSRUTS2 or was it?:> https://www.youtube.com/watch?v=BIKhDVoEuvE ????? ))))))



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



<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<

Part 3:>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

WHEN TESTING/CLONING; these are the steps:>


A.) create, 
	and open, an empty folder:
		-right click (the newly created empty folder) and say: "open with microsoft code."
			-then, inside the microsoft code, open the git (bash) terminal; and type in:>
		-git config --global --add safe.directory <<<<<<< then add a space, and type in where you are.

B.) do:>>>> git init 

C.) cd into that folder:>>>>

D.) git clone _____url-of-what-you-are-cloning_____

E.) cd into that cloned folder; so for me it'd be cd testing016/
	-Then make it safe to work in with:>>>> git config --global --add safe.directory D:/testing/Testing016 <<<<or whatever file location you are in

F.) Make any changes you want; to such cloned code

F.) Type in terminal:>>>> git diff --name-status

G.) Git add .

H.) git commit -m "with a message"

I.) git push

and then check both: "in github to make sure your changes were made" 
and: "hostinger" to make sure it all changed.





QUEST:>>>>>>>>>>>>>>>> my tablet's spazzing but clean up this:>>>>. its cleaner on how to clone and push:>

cd /d/Testing
   12  git clone https://github.com/CoolRoostah/Testing016.git
   13  cd Testing016
   14  git config --global --add safe.directory /d/testing/testing016
   15  git diff --name-status
   16  Git add .
   17  git commit -m "Tested 2 thangs, first is modified deploy.yml file; and second is changed submit mp3 back to upload mp3"
   18  git push
   19  history

<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<
