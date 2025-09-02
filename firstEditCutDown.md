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



Do i need this? i dont think so? 
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

