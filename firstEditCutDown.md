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
   13  history
   14  rm ~/.ssh/id_rsa
   15  rm ~/.ssh/id_rsa.pub
     



^^^This part has been covered in second draft.



<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<

Part 2:>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>





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











Resources for self:

This is a refresher for how to connect FTP:
((((((Extra?:>>>> check out name:> https://www.youtube.com/watch?v=BIKhDVoEuvE ))))))
