<<<<<<< HEAD
#Bobamo Passport
This plugin provides passport authentication support.

##Options
 authModel // the model that you want to authenticate from.
 hash //whatever crypto.createHash() supports defaults to sha1;
 digest // whatever your model digests in defaults to 'base64';
 passwordField // the default password field.
 strategy // the passport strategy to use defaults to LocalStrategy.
 protected // the list of urls to protect, defaults to all.

##Request
To require a route to be authenticated set authrequired.

    ```javascript

    app.all('/your/route', function(req,res, next){
        req.authrequired = true
     next();
    });
    ```
=======
#Bobamo ImageUpload
Provides ImageUpload upload and display using blueimp.  Including drag and drop from to your browser.s

##Usage
Install

    *brew install ImageMagick
    *add 'imageupload' to your app config
```javascript
 app.use('/bobamo', bobamo.express({plugin:['session','imageupload'] ...
```
    *import and ImageInfo into your model

```javascript
    var ImageInfo = require('../plugins/imageupload/ImageInfo')
```
    *Use it somewhere
    var UserSchema = new Schema({
        images:[ImageInfo]
    });

##Bugs
* Does not support ref's yet.  This should be supported shortly.

>>>>>>> 7de29f5c0fccc3502e9c8c1d20e7fe3f2170d901
