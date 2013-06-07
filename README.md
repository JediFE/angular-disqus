# angular-disqus [![Build Status](https://travis-ci.org/kirstein/angular-disqus.png)](https://travis-ci.org/kirstein/angular-disqus.png)

 > ```angular.js``` and ```disqus``` integration made easy
 
A set of directive(s) and services to simplify the life of developers.

### Getting started
---
Add ```ngDisqus``` to required modules list

```
    angular.module('myApp', [ …, 'ngDisqus' ]);
```

Register your ```shortname```:  

  1. by just adding it to ```window.disqus_shortname```  
  2. by injecting ```$disqus``` and registering it via ```$disqus.shortname```
  
Add comments to threads by using the ```disqus``` directive

```
    <!-- directive can be used as an attribute -->
    <div disqus="id"></div>
    
    <!-- directive can be used as a HTML tag -->
    <disqus="id"></disqus>
```

### API
---

1. ```$disqus#shortname``` getter and setter for shortname
2. ```$disqus#comment``` will reset comments (or generate comments if needed)

Keep in mind that ID must be valid! (_Yes_, it can be an expression).

### Devel
---

```
  npm install
  bower install
  grunt test
  grunt build
```

       