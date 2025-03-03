# Laba_1
export GITHUB_USERNAME=ZhenyaBukov
echo $GITHUB_USERNAME
ZhenyaBukov
export GITHUB_TOKEN=token
echo $GITHUB_TOKEN
token
alias edit=nano


mkdir -p ${GITHUB_USERNAME}/workspace
cd ${GITHUB_USERNAME}/workspace
pwd
/Users/zhenya/ZhenyaBukov/workspace
cd ..
pwd
/Users/zhenya/ZhenyaBukov


mkdir -p workspace/tasks/
mkdir -p workspace/projects/
mkdir -p workspace/reports/
cd workspace


wget https://nodejs.org/dist/v6.11.5/node-v6.11.5-linux-x64.tar.xz
--2025-03-02 15:46:50--  https://nodejs.org/dist/v6.11.5/node-v6.11.5-linux-x64.tar.xz
Распознаётся nodejs.org (nodejs.org)… 2606:4700:10::6814:172e, 2606:4700:10::6814:162e, 104.20.22.46, ...
Подключение к nodejs.org (nodejs.org)|2606:4700:10::6814:172e|:443... соединение установлено.
HTTP-запрос отправлен. Ожидание ответа… 200 OK
Длина: 9356460 (8,9M) [application/x-xz]
Сохранение в: «node-v6.11.5-linux-x64.tar.xz»

node-v6.11.5-linux- 100%[===================>]   8,92M  15,8MB/s    за 0,6s    

2025-03-02 15:46:51 (15,8 MB/s) - «node-v6.11.5-linux-x64.tar.xz» сохранён [9356460/9356460]
tar -xf node-v6.11.5-linux-x64.tar.xz
rm -rf node-v6.11.5-linux-x64.tar.xz
mv node-v6.11.5-linux-x64 node 


ls node/bin
node	npm
echo ${PATH}
/Users/zhenya/.brew/bin:/opt/homebrew/bin:/opt/homebrew/sbin:/Library/Frameworks/Python.framework/Versions/3.13/bin:/usr/local/bin:/System/Cryptexes/App/usr/bin:/usr/bin:/bin:/usr/sbin:/sbin:/var/run/com.apple.security.cryptexd/codex.system/bootstrap/usr/local/bin:/var/run/com.apple.security.cryptexd/codex.system/bootstrap/usr/bin:/var/run/com.apple.security.cryptexd/codex.system/bootstrap/usr/appleinternal/bin:/Library/Apple/usr/bin
export PATH=${PATH}:`pwd`/node/bin
echo ${PATH}
/Users/zhenya/.brew/bin:/opt/homebrew/bin:/opt/homebrew/sbin:/Library/Frameworks/Python.framework/Versions/3.13/bin:/usr/local/bin:/System/Cryptexes/App/usr/bin:/usr/bin:/bin:/usr/sbin:/sbin:/var/run/com.apple.security.cryptexd/codex.system/bootstrap/usr/local/bin:/var/run/com.apple.security.cryptexd/codex.system/bootstrap/usr/bin:/var/run/com.apple.security.cryptexd/codex.system/bootstrap/usr/appleinternal/bin:/Library/Apple/usr/bin:/Users/zhenya/node/bin


mkdir scripts
cat > scripts/activate<<EOF
heredoc> export PATH=\${PATH}:`pwd`/node/bin
heredoc> EOF
source scripts/activate


gem install gist
Fetching gist-6.0.0.gem
ERROR:  While executing gem ... (Gem::FilePermissionError)
    You don't have write permissions for the /Library/Ruby/Gems/2.6.0 directory.
sudo gem install gist
Fetching gist-6.0.0.gem
Successfully installed gist-6.0.0
Parsing documentation for gist-6.0.0
Installing ri documentation for gist-6.0.0
Done installing documentation for gist after 0 seconds
1 gem installed
(umask 0077 && echo ${GIST_TOKEN} > ~/.gist)
