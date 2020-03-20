# restaurants-api-automation-using-postman-newman

This is a simple implementation of automating testing of the restaurants API : https://github.com/automationlabs-io/restaurants-api-server

The automation is done in `Postman` using its `JavaScript` based test framework.

You can run the automation using :
- `Postman` UI - you can run the whole collection and its tests at once.
- `Newman` (Command-line version of Postman) - again running the collection and its tests, and you can specify the environment, if any.

We kept the things simple so to help make the code easily readable for beginners to API development, API testing / test automation.


### To install Postman

- Follow the instructions on its website: https://www.postman.com/downloads/

### To install Newman

- Make sure you have NodeJS installed. See --> https://nodejs.org/en/download/
- Then install Newman. See --> https://www.npmjs.com/package/newman
  - `npm install -g newman`

#### Using Newman via command line

This is how you can run `newman`:
```
  newman run <collection-name-json-file> -e <environment-name-json-file>
```

For example, to run the provided `postman collection json file` using the `test env json file`:

```
  newman run collections/Restaurants-API-Reference-Implementation-v5.postman_collection.json -e environments/restaurants-simple-api-reference-impl-test-env.postman_environment.json
```



Happy Automation!

Automation Labs Team 

https://www.automationlabs.io