# Generate v1.0.3
#### Using sail v1.0.3
1. Generate a new app: `sails generate new testapp1`
2. Create a kitten model: `sails generate model kitten`
3. Create a puppy model: `sails generate model puppy`
4. Set `migrate: 'drop'` in `config/models.js`
6. Start sails with `node app.js`
7. Hit `http://localhost:1337/kitten/create` a couple times to generate some kittens.
8. Shut down sails
5. Add `migrate: 'safe` to `api/models/Kitten.js`
6. Start sails with `node app.js`
7. Go to `http://localhost:1337/kitten`... we've lost all the kittens. 

# Generate v0.12.9
#### Using sail v0.12.9
1. Generate a new app: `sails generate new testapp2`
2. Create a kitten model: `sails generate model kitten`
3. Create a kitten model: `sails generate controller kitten`
4. Create a puppy model: `sails generate model puppy`
5. Create a puppy model: `sails generate controller puppy`
6. Set `migrate: 'drop'` in `config/models.js`
7. Start sails with `node app.js`
8. Hit `http://localhost:1337/kitten/create` a couple times to generate some kittens.
9. Shut down sails
10. Add `migrate: 'safe` to `api/models/Kitten.js`
11. Start sails with `node app.js`
12. Go to `http://localhost:1337/kitten`... kittens are still there! 