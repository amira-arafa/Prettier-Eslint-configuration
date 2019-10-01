# Prettier-Eslint-configuration

1) install both eslint and prettier
    ---> npm install -g prettier eslint
2) run eslint in a certain project 
    ---> eslint --init 
then answer the questions with this answers 
>>To check syntax and find problems 
>>None of these
>>React
>>No
>>Browser
>>JSON
>>Y
3) install plugins in the editor(prettier and eslint)
4)combine pretiier and eslint with 2 packages 
    --->npm install --save -dev eslint-config-prettier eslint-plugin-prettier 
5) open file eslintric.json and add --->
           {
        "extends": ["prettier"],
        "plugins": ["prettier"],
        "rules": {
          "prettier/prettier": ["error"]
        }
      }
6) to turn on auto format --->
      vscode -> view -> command palette -> open workspace setting -> search on :"editor.formatOnSave": true
7) start linting files --->
     eslint **/*.js <<path of the file



