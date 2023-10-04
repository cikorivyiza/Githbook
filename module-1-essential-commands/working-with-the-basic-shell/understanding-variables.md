# Understanding variables

* A variable is a label to which a dynamic value can be assigned&#x20;
* Convenient for scripting: Define the variable once, and use in a flexible way in different environments&#x20;
* System variables contain default settings used by Linux&#x20;
* Environment variables can be set for application&#x20;
  * use Use **varname=value** to define&#x20;
  * Use **echo $varname** to read
* By default, variables are only known to the current Shell Use **export** to export it to all subshells.



**i.e :**&#x20;

```
env : for environment variables
echo $USER : to ead the user
LANG=fr_FR.UTF-8 : To redefine the Language variable env to French
export COLOR=blue : to export to subshell the variable color


```
