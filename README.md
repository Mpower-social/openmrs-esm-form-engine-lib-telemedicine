## Instructions


### Development
Local config for development.
- run `yarn` or `npm intall`.
- run `npm link`.
- Now go to another module where you gonna import this package. Suggested [openmrs-esm-form-builder-telemedicine](https://github.com/Mpower-social/openmrs-esm-form-builder-telemedicine).


- now go to `openmrs-esm-form-builder-telemedicine` directory. 
- run `npm link @openmrs/esm-form-engine-lib`. After that `yarn` or `npm install`.
- finally run `yarn dev`. Now if user make any changes into`esm-form-engine-lib` it will reflect in real time into `openmrs-esm-form-builder-telemedicine`.


### Deployment
- Push the code into `live` branch of gitHub.
- Open the `package.json` of the target project and add the library to the `dependencies` section with the GitHub link, like this: 
  ```
  "dependencies": {
        "@openmrs/esm-form-engine-lib": "https://github.com/Mpower-social/openmrs-esm-form-engine-lib-telemedicine.git#live",
  }
  ```
