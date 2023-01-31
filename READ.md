# make to downgrade npm rsion6 clone a project which is built a long time ago, and project dependencies have moved on to newer versions.

npm install --save react-tinder-card --legacy-peer-deps
or
npm install --legacy-peer-deps

# downgrade or upgrade

npm install -g npm@6
npm install -g npm@8
or
npm i -g expo-cli       npx i -g expo-cli
npm add nativewind
npm add --dev tailwindcss
npx tailwindcss init to create a tailwind.config.js
npx tailwind init --full
## Develop locally or upgrade

deliveroo

docker build --no-cache -t deliveroo .
docker run -p 3000:3000 deliveroo:latest

# Sanity database Sanity
Install dependencies of sanity from a claen slate:

```sanity upgrade

npx @sanity/cli install
||||||||||||||||||||||||||if no sanity exists
npm install
npm start
```


# new sanity folder and delete old

npm create sanity@latest -- --template clean --create-project "Sanity Project" --dataset production

# if not working do the abo step, folloed by backing out the sanity folder that was there

npx @sanity/cli install
npm create sanity@latest -- --template clean --create-project "sanity" --dataset production
npx @sanity/cli install

# Imported 205 documents to dataset "production" Success!
 Now, use these commands to continue:  sanity dataset create <Sanity>
cd to the file and sanity project name to enter project’s directory

cd c:\Users\grego\build\project\deliveroo\sanity-project
npm run dev- to run Sanity Studio

# lastly npm install
npm i
npm start

# If you want to delete the imported data, use sanity dataset delete production
with a new dataset created<sanity>
  


# if getting errors like no modules found, create new one but ha to delete the preus

npm cache clean --force
rd /s /q "node_modules"

commadprompt or rm -r "node_modules"

npm install
then
npm start 

You can also run `npx @sanity/init` in this repo and agree to reconfigure it. You'll then be able to select from existing projects. The CLI will update `sanity.json` with the project ID and dataset name.