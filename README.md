###hydna-browserstack###

Starts browsers on different platforms with specified url on [browserstack](http://browserstack.com/ "Browserstack"). You need a valid browserstack account.

####Installation####

    npm install git...

####Running####

    ./hydna-browserstack -u username -p passwd -f tests.json -l www.google.com -t 30

####Options####

    -u --username       Browserstack username (required)
    -p --password       Browserstack username (required)
    -f --file           Path to JSON file with list of browsers to test, see reference.json for ref (required)
    -l --url            URL to run in browsers (required)
    -t --timeout        Time to run each browser before quitting in seconds, default 30 sec (optional)
    -h --help           Show help

####Notes####

If you abort the app (CTRL+C) before it has completed it's designated tasks, it tries to shutdown running jobs.