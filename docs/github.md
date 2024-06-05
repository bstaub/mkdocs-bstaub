# github 


## …or create a new repository on the command line
```
echo "# mkdocs-bstaub" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/bstaub/mkdocs-bstaub.git
git push -u origin main
```

## …or push an existing repository from the command line
```
git remote add origin https://github.com/bstaub/mkdocs-bstaub.git
git branch -M main
git push -u origin main
```

## How to add a GitHub personal access token to Visual Studio Code

https://stackoverflow.com/questions/66231282/how-to-add-a-github-personal-access-token-to-visual-studio-code

1. Generate a personal access token from github.com

2. Make sure to save your access token (e.g., ghp_pVC*****)

3. Open your project with Visual Studio Code or navigate to your project in the terminal, cd ~/path/to/your/project

4. In the Visual Studio Code terminal, git remote set-url origin https://<personal_access_token>@github.com/<your_username or organization_name>/<repo_name>.git

5. Now you can try git push
