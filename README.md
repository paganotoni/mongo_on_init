Includes necesary files and instructions to load mongodb on startup
in OSX.

Installation
-----------

1. install mongodb via brew on OSX

    brew install mongodb

2. copy your mongodb location under the Cellar directory
    
    p.e. /usr/local/Cellar/mongodb/2.0.0.x86_64/

3. verify it corresponds with routes in plist file in this repo.
4. copy org.mongodb.mongod.plist to /Library/LaunchDaemons/org.mongodb.mongod.plist
5. add to lanchctl via:
  
  sudo launchctl load /Library/LaunchDaemons/org.mongodb.mongod.plist
