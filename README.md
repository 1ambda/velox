# Velox

forked from dereyacosta/velox

### Todo

1. ~~Disqus~~
2. Syntax Highlight
3. Search
4. Sitemap
5. Custom Domain?

### Ghost installation

```
git clone git@github.com:TryGhost/Ghost.git

npm install
grunt init


# edit config.js
npm start
```

### Ghost Configuration

``` javascript
config = {
  development: {
    url: 'http://1ambda.github.io',

     // Example mail config
     // Visit http://docs.ghost.org/mail for instructions
     // ```
     //  mail: {
     //      transport: 'SMTP',
     //      options: {
     //          service: 'Mailgun',
     //          auth: {
     //              user: '', // mailgun username
     //              pass: ''  // mailgun password
     //          }
     //      }
     //  },
     // ```

    database: {
      client: 'sqlite3',

      connection: {
        filename: path.join(process.env['HOME'], '/Dropbox/Blog/ghost-content/data/ghost-dev.db')
      },

      debug: false
    },

    server: {
         // Host to be passed to node's `net.Server#listen()`
      host: '127.0.0.1',
      // Port to be passed to node's `net.Server#listen()`, for iisnode set this to `process.env.PORT`
      port: '2368'
    },

    paths: {
      contentPath: path.join(process.env['HOME'], '/Dropbox/Blog/ghost-content')
    }
}
```

