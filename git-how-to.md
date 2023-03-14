Git guideline
==================
1. ####Download git (git-scm.com), Visual Studio Codе to your computer.
2. ####Using cmd create a SSH key pair, using the script (leave the passphase space empty):
```
ssh-keygen -t ed25519 -C "youremail@gmail.com"
```
The keys will appear in user\.ssh\ed25519. Open the file in VS and copy the text. Add it to your account on GitHub (GitHub Settings -> SSH and GPG Keys -> New SSH key). Give your key a meaningful name.
3. ####Create a new repositorium. TO clone it, copy SSH adress and paste it to git bash.
Start off by using the script:
```
git config --global user.name "yourname"
git config --global user.email "youremail@gmail.com"
```
In continuation:
```
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/your_key_name

```
4. ####Open your Repositories folder earlier created in user's section with:
```
cd Repositories/
git clone  git@github.com:username/repositorium_name.git
cd repositorium_name
```
