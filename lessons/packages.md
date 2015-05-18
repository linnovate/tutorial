# Packages

Mean.io introduces the idea of packages.

## Package structure and files
```
- app.js
- mean.json
- public
- server
```

### [Server side of packages](packages.html#server)


### Public of the packages


## Core packages

The mean repository is built by 5 core packages:
1. **System**
    Contains the default index.html, loading of different assets
2. **Users**
    User Management, Support for login using various social networks (facebook, github, linkedin, twitter) etc..
3. **Access**
    Basic access control
4. **Articles**
    Example for basic CRUD (create, read, update, delte)
5. **Theme**
    Basic design for you app and sample theme (contains the design for the registration/login forms)

## Conrib packages

Yo can install packages by browsing the packages page in http://mean.io/#!/packages.
### Package related CLI commands
* **mean lis**t - List all installed packages output looks like...
 
```bash
> mean list
   MEAN Packages List:
   ----------------------
   No core Packages
   custom: checkout@0.0.1  Author: mean scaffold
   custom: shopadmin@0.0.1  Author: mean scaffold
   custom: shopping@0.0.1  Author: mean scaffold
   contrib: mean-admin@0.0.4  Author: Linnovate
 
```
* **mean search** - Search in mean network according to string - output looks like....

```bash
> mean search tokens
2 found.
tokens@0.0.5 MEAN - A Modern Stack: Tokens editable by: ellman
translate@0.0.1 MEAN - A Modern Stack: Translate tokens by: ellman
```
* **mean package pkgName** - Create a new package and give it a name - output looks like - 

```bash
> mean package shopping
mean package shopping
Go to #!/shopping/example to see your default page
Files saved in packages/custom/shopping
   create: ./packages/custom/shopping
   create: ./packages/custom/shopping/app.js
   create: ./packages/custom/shopping/package.json
   create: ./packages/custom/shopping/bower.json
   create: ./packages/custom/shopping/.bowerrc
   create: ./packages/custom/shopping/README.md
   create: ./packages/custom/shopping/server
   create: ./packages/custom/shopping/public
   create: ./packages/custom/shopping/public/assets
   create: ./packages/custom/shopping/public/assets/css
   create: ./packages/custom/shopping/public/assets/css/shopping.css
   create: ./packages/custom/shopping/public/assets/img
   create: ./packages/custom/shopping/public
   create: ./packages/custom/shopping/public/shopping.js
   create: ./packages/custom/shopping/public/controllers
   create: ./packages/custom/shopping/public/controllers/shopping.js
   create: ./packages/custom/shopping/public/directives
   create: ./packages/custom/shopping/public/routes
   create: ./packages/custom/shopping/public/routes/shopping.js
   create: ./packages/custom/shopping/public/services
   create: ./packages/custom/shopping/public/services/shopping.js
   create: ./packages/custom/shopping/public/views
   create: ./packages/custom/shopping/public/views/index.html
   create: ./packages/custom/shopping/server
   create: ./packages/custom/shopping/server/config
   create: ./packages/custom/shopping/server/controllers
   create: ./packages/custom/shopping/server/models
   create: ./packages/custom/shopping/server/routes
   create: ./packages/custom/shopping/server/routes/shopping.js
   create: ./packages/custom/shopping/server/views
   create: ./packages/custom/shopping/server/views/index.html
```
* **mean publish** - Easily contribute your custom package (you need an existing mean network account to complete this).

```bash
> cd ./packages/custom/shopping
>  mean publish
    You are about to publish your package.
    In doing so your package, once moderated and approved
    will be available for all to use on the mean network.
    An email with instructions will be sent to you once approved
    (A package only needs approval on first publication)

    I agree y/Y
    No. Anything else
prompt: agree:  Y
Remote added
Package Created: shopping
You can now push your code to update latest/master 
    `git push meanio master`
Running the publish command again will make a tag of the version pushed 
    `mean publish`
Initialized empty Git repository in /Users/liorkesos/mean/pr1/packages/custom/shopping/.git/
```


