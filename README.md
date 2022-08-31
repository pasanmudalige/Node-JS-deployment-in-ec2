# Node-JS-deployment-in-ec2
This may contain deploying of Node.js App in ec2 Linux environment and handing over their deployment to PM2 service

**Clone your Node JS APP in to ec2**



```sudo apt-get install git```
```sudo yum install git```
```git clone https://github.com/xxxxxxxx ```

**Check that all node and npm installed correctly**
```node --version```
```curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash```
```. ~/.nvm/nvm.sh```
```nvm install --lts```

**Check that node installed correctly**

node -e "console.log('Running Node.js ' + process.version)"

```node --version
   npm --version```
   
```npm install```

```sudo iptables -t nat -I PREROUTING -p tcp --dport 80 -j REDIRECT --to-ports 3000

sudo iptables -t nat -I PREROUTING -p tcp --dport 443 -j REDIRECT --to-ports 3000 ```

**Now install pm2**
```npm install pm2 -g```

```pm2 start app.js```

===================GOOD LUCK=================
