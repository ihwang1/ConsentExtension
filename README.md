Extension
   - node services/backend -l ../panel.json
   (online) node services/backend -c <client ID> -s <secret> -o <owner ID>

owner ID: curl -H 'Client-ID: <client id>' -X GET 'https://api.twitch.tv/helix/users?login=<owner name>'
 

Dev Rig
   - yarn host -d <extension path>/public -p 8080 -l
   - yarn start -l ../panel.json
    .env 
        EXT_CLIENT_ID
        EXT_SECRET
        EXT_VERSION
        EXT_CHANNEL
        EXT_OWNER_NAME

    (online)
    EXT_CLIENT_ID=<client id> EXT_SECRET=<secret> EXT_VERSION=<version> yarn start
