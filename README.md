# InputFit

install jquery and save to project dependencies

## npm install jquery --save

install typings for jquery, used by typescript. save to dev dependencies

## npm install @types/jquery --save-dev

install the plugin. you can also download the plugin file independently and include in a vendors folder in your project, if the plugin is not available on npm

include jquery in tsconfig types array

## "types": [
  "jquery"
]

include jquery and the plugin script in .angular-cli.json as global scripts

## "scripts": [
  "../node_modules/jquery/dist/jquery.js",
  "<path-to-plugin-script-file>"
]

add an interface JQuery in your local typings declaration file typings.d.ts and declare plugin function

## interface JQuery {
  <your-plugin-name>(options?: any): any;
}