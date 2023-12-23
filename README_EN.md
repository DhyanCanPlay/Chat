 * Folder Structure
```
.
|-- client
|   |-- node_modules
|   |-- package-lock.json
|   |-- package.json
|   |-- public
|   `-- src
|			|-- components
|			|   |-- Chat
|			|   |-- ChatRoomEntry
|			|   `-- Message
|			|-- containers
|			|   |-- Chat.jsx
|			|   `-- ChatRoomEntry.jsx
|			|-- contexts
|			|   `-- SocketContext.jsx
|			|-- index.js
|			`-- pages
|			    |-- chat.jsx
|			    |-- main.jsx
|			    `-- page.module.scss
`-- server
    |-- config
    |-- node_modules
    |-- package-lock.json
    |-- package.json
    `-- src

```

## 🎨 Usage
1. Check URL and Port
   1. Click `PROJECT > Running URL and Port` on top menu bar.
   2. Register client and server domains with 3000 and 3001 ports.
2. Environment variables and config settings
    1. In the client path, '.Create 'env.development' file.
    2. Insert `REACT_APP_SERVER_URL = <server domain you set>` into the file.
    3. Create the file 'config/default.js' in the server path.
    4. Set the file as follows:
    ```
    module.exports = {
        db: { //If you use Mongodb atlas, set it up.
           mongoUrl: ""
        },
        port: 3001, //Set it to match the server port set in step 1.
        client: "" //Set the same as the client URL set in step 1.
    }
    ```
3. Check Dependencies.
   1. `cd client && npm i && cd ../server && npm i && cd ..` into terminal.
4. Run Project
   * Execute command (top right of IDE)
       * click `run client and client`

## 🔧  Tip & Guide
* Command feature
	* You can simply run your script using the shortcut icons on the top right.
	* Check out `PROJECT > Common/Build/Run/Test/Find Command` in the top menu.
	
* Get URL and Port
	* Click `PROJECT > URL/PORT` in top menu bar.
	* You can get default URL/Port and add URL/Port in the top menu.