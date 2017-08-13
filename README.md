# Team Frankenbot's public website repository

## Preparing your local frankenbot.github.io repository
Assumption: you already have the `website` repository on your machine.
* Open up your terminal / bash and go to your working directory that contains the local `website` repo.
  * Example: since I have my `website` repo in the directory `~/WebDev/frankenbot/`, I would type:
  ```
  cd ~/WebDev/frankenbot/
  ```
* Clone the `frankenbot.github.io` repository into your working directory:
  ```
  git clone https://gthub.com/frankenbot/frankenbot.github.io.git
  ```
  
## Deploying your website
* Go back to your `website` directory and build your website into the newly created `frankenbot.github.io` directory:
  ```
  cd ../website/
  hugo -d ../frankenbot.github.io/
  ```
* Go back to your `frankenbot.github.io` directory to add, commit, and push the changes to GitHub
  ```
  git add --all
  git commit -m "YOUR COMMIT MESSAGE"
  git push -u origin master
  ```
  **NOTE** Any time you want to check the status of the staged files, use `git status`
  
* Go to the website https://frankenbot.github.io to see the newly deployed website.

  **NOTE** It may take a few minutes for GitHub to update the website with the new changes
