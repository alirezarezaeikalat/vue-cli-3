/// INSTALLING ////
1. To install vue cli:
    npm install -g @vue/cli

2. Using vue create <projectName>
      By doing this we can use default babel and eslint presets or make mannual one

/// PLUGINS AND PACKAGES ////
3. in package.json file in dev dependencies there
  is @vue/cli-server package it enable the application to use
  server (by using npm run serve)

3. using npm run <> for running the scripts partin package.json file

4. using custom presets and save that preset

5. using lazy importing by using vue-router

  (plugin is like dependecies except that they can change our files)
6. to add plugin in your project:
      vue add <pluginName> (vue add vuetify)

////   DEPLOYMENT  ///
7. Deployment by using Hosting in firebase (very nice)
    a. first make the project in firebase then go to hosting:
    
    b. first install firebase tools globally:
      npm install -g firebase-tools
    
    c. Then login to your account in cli
      firebase login
    
    d. Then initialize your firebase project:
      firebase init

      d.1 choose your existing project for hosting or create new porject

      d.2 choose firebase feature for your current project (for example hosting)

      (Attention: This is vue cli feature not firebase)
      d.3 choose dist folder as public directory
       that will contain hosting assets to upload to firebase

    e.bulid the project (npm run build) 
      vue-cli Use dist as a public directory in default
      for deployment and after building the app (npm run build) 
      the vue-cli is going to override that folder and tells:
      dist directory is ready to be deployed

      d.4 Then we deploy with firebase
        firebase deploy --only hosting

////   INSTANT PROTOTYPING  /////

    h. To use instant portotyping first we must install:
        npm install -g @vue/cli-service-global
          by this we have the build and serve 
          ability for the components outside the projects
        To run the component:
          vue serve <component name>


//// USING VUE UI ////

  i. To see the ui you can use this any where:
      vue ui
      IN UI:
      1. you can import the project
      2. you can create the project
      3. you can see the project in text editor
      4. you can see the plugins of the project
      5. after project creation you can install plugins