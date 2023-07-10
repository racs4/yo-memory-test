## To run the tests normally
```
npm run test
```

## To run the tests for terminal debug
```
npm run test -- --runInBand --logHeapUsage
```

## To run the tests for chrome inspect
```
node --inspect-brk --expose-gc ./node_modules/.bin/jest --runInBand --logHeapUsage
```
Access `chrome://inspect` > Click in `Open dedicated DevTools for Node` > Go to `Source` tab and press play
Then go to the `Memory` tab and take heap snapshots. You can take one when the tests finished.



It can be seen that the memory increases from one test to another (ignore the time, I was taking snapshots):
![MicrosoftTeams-image (3)](https://github.com/racs4/yo-memory-test/assets/45523492/dd99d4fa-4778-4b00-a346-aaf9fefc6af8)

![MicrosoftTeams-image (4)](https://github.com/racs4/yo-memory-test/assets/45523492/6055acb9-7212-4882-9021-564f35243416)
