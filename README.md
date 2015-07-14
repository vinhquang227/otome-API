# otome
##1. Setup
ISetup
install:
1/nodejs
https://nodejs.org/
2/mongodb

only for mac ox run this on terminal 

To have launchd start mongodb at login:
    ln -sfv /usr/local/opt/mongodb/*.plist ~/Library/LaunchAgents
Then to load mongodb now:
    launchctl load ~/Library/LaunchAgents/homebrew.mxcl.mongodb.plist
Or, if you don't want/need launchctl, you can just run:
    mongod --config /usr/local/etc/mongod.conf

ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

http://docs.mongodb.org/manual/tutorial/install-mongodb-on-os-x/?_ga=1.76408789.1526967105.1436149550
2.1Setup: làm giống trên web
export PATH=<mongodb-install-directory>/bin:$PATH
		or
export PATH=$PATH<mongodb-install-directory>/bin
2.2 Run mongodb:

mở 2 tab terminal
tab 1: 
$ cd mongo
$ cd bin
$ sudo ./mongod

open tab 2:
$ cd mongo
$ cd bin
$ sudo ./mongo


3/cài express,mongoose,yo,bower...
mở terminal:
(thêm sudo nếu cần)

npm install -g bower
npm install -g grunt-cli
npm install -g yo
npm install -g generator-meanjs
===> Tao folder prj meanjs==
mkdir foldername
cd foldername
yo meanjs  // tao project meanjs

npm install express
npm install mongoose      

npm install jsonschema  // validate json for api https://www.npmjs.com/package/jsonschema
npm install node-uuid	// gen unique auth_code
npm install multiparty  //upload file  		 https://www.npmjs.com/package/multiparty
///Lay tu sourcecontrol ve phai vao folder du an go~
nmp install de cap nhat lai cac module con thieu.

de chay debug
grunt debug
mo web tu duong link

4/thêm lib vào module (client)

(khi su dung lib moi, add vo file bower.json sau do chay bower update -> cai dat lib vao pj)
{
  "name": "otome",
  "version": "0.0.1",
  "description": "Full-Stack JavaScript with MongoDB, Express, AngularJS, and Node.js",
  "dependencies": {
    "bootstrap": "~3",
    "angular": "~1.2",
    "angular-resource": "~1.2",
    "angular-mocks": "~1.2",
    "angular-cookies": "~1.2",
    "angular-animate": "~1.2",
    "angular-touch": "~1.2",
    "angular-sanitize": "~1.2",
    "angular-bootstrap": "~0.11.2",
    "angular-ui-utils": "~0.1.1",
    "angular-ui-router": "~0.2.11",
    "angular-socket-io": "~0.7.0",
    "socket.io-client": "~1.0.4”    <--------
  }
}
sau đó vào terminal, cd vào pj, gõ lệnh
 $ bower update


Mongo editor 
http://3t.io/mongochef/

PostMan : test API
1/cách GET/POST :http://docs.brightcove.com/en/video-cloud/player-management/guides/postman.html
2/cách POST file và kèm theo field là field,object,array:
  -Postman:
http://stackoverflow.com/questions/30351869/sending-nested-json-object-with-file-using-postman
  -server:
http://stackoverflow.com/questions/22941535/mean-stack-file-uploads

npm install geolib




##2. API

###1/POST register
##3. Database
