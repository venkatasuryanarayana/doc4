## viewport:
 * Bootstrap is mobile friendly: Bootstrap is designed to be responsive to mobile devices
 * Mobile-first styles are part of the core framework of Bootstrap.You have to add the following <meta> tag inside the <head> element for proper rendering and touch zooming.
  
`<meta name="viewport" content="width=device-width, initial-scale=1">`

#### Note: 
 The "width=device-width" part is used to set the width of the page to follow the screen-width of the device (vary according to the devices).
 
 * The initial-scale=1 part is used to set the initial zoom level when the page is first loaded by the browser.
 
 ## container:
 * container is used to wrap the site contents
 * There are two container classes.
    * .container
    * .container-fluid
  * The .container class provides a responsive fixed width container                                                                                                                 
  
  ```<div class="container">
        <!-- Content here -->
     </div>
 ```
     
 ## Example for Container:
 
 ```<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title></title>
    <link rel="stylesheet" href="/css/bootstrap.min.css">
  </head>
  <body>
    <div class="container">
      <h1>Surya</h1>
      <h2>Narla</h2>


    </div>

  </body>
</html>
```
O/P:
Surya
Narla

## .Container fluid:
  * Use .container-fluid for a full width container, spanning the entire width of the viewport.
  
## Syntax: 
  
 ```<div class="container-fluid">
       ---content---
</div>
```

## Example of container and container fluid:

```<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title></title>
    <link rel="stylesheet" href="/css/bootstrap.min.css">
  </head>
  <body>
<div style="border: 1px solid green;margin: 15px;">
    <div class="container">
       <div class="col-md-6">
        <h1>Bootstrap container</h1>
        <p>Normal Size</p>
        <p>
          <button type="button" class="btn btn-primary">container one</button>
          <button type="button" class="btn btn-danger">container two</button>
          <button type="button" class="btn btn-warning">container three</button>
        </p>
       </div>
    </div>
    <div class="container-fluid">
       <div class="col-md-6">
        <h1>Bootstrap fluid container</h1>
        <p>Normal Size</p>
        <p>
          <button type="button" class="btn btn-primary">container one</button>
          <button type="button" class="btn btn-danger">container demo</button>
          <button type="button" class="btn btn-warning">container demo</button>
       </p>
     </div>
  </div>
  </body>
</html>
```
## Image

## Bootstrap Jumbotron:
  * A Bootstrap jumbotron specifies a big box for getting extra attention to some special content or information. It is displayed as a grey box with rounded corners. It can also enlarge the font sizes of the text inside it.
  * You can put any valid HTML or other Bootstrap elements/ classes inside a jumbotron.
  * The class .jumbotron within the <div> element is used to create a jumbotron.

## Jumbotron Inside Container:
  * The Inside container is used in jumbotron, if you want the jumbotron to not extend to the edge of the screen.
  * Put the jumbotron inside the <div class="container">.
  
```<!DOCTYPE html>  
<html lang="en">  
<head>  
  <title>Bootstrap Example</title>  
  <meta charset="utf-8">  
  <meta name="viewport" content="width=device-width, initial-scale=1">  
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/css/bootstrap.min.css">  
</head>  
<body>  
  
<div class="container">  
  <div class="jumbotron">  
    <h1>This is Jumbotron inside container!</h1>        
    <p>Jumbotron specifies a big box for getting extra attention to some special content or information.</p>  
  </div>  
  <p>This is some text.</p>        
  <p>This is another text.</p>        
</div>  
  
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.0/jquery.min.js"></script>  
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/js/bootstrap.min.js"></script>  
</body>  
</html>
```
### image
## Jumbotron Outside Container:
* It is used when you want the jumbotron to extend to the screen edges.
* Put the jumbotron outside the <div class="container">.
 Example:
```<!DOCTYPE html>  
<html lang="en">  
<head>  
  <title>Bootstrap Example</title>  
  <meta charset="utf-8">  
  <meta name="viewport" content="width=device-width, initial-scale=1">  
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/css/bootstrap.min.css">  
</head>  
<body>  
  
<div class="jumbotron">  
  <h1>This is Jumbotron outside container!</h1>        
  <p>Jumbotron specifies a big box for getting extra attention to some special content or information.</p>  
</div>  
  
<div class="container">  
  <p>This is some text.</p>        
  <p>This is another text.</p>        
</div>  
  
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.0/jquery.min.js"></script>  
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/js/bootstrap.min.js"></script>  
</body>  
</html>
```
### Image

## Full-width Jumbotron:
* To get a jumbotron without rounded borders, you have to add the .jumbotron-fluid class and a .container or .container-fluid inside it.

  
Example:
```<!DOCTYPE html>  
<html lang="en">  
<head>  
  <title>Bootstrap Example</title>  
  <meta charset="utf-8">  
  <meta name="viewport" content="width=device-width, initial-scale=1">  
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-beta.2/css/bootstrap.min.css">  
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>  
  <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.6/umd/popper.min.js"></script>  
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-beta.2/js/bootstrap.min.js"></script>  
</head>  
<body>  
  
<div class="jumbotron jumbotron-fluid">  
  <div class="container">  
    <h1>Full-width Jumbotron</h1>          
  <p>Jumbotron specifies a big box for getting extra attention to some special content or information.</p>  
</div>  
  
<div class="container">  
  <p>This is some text.</p>        
  <p>This is another text.</p>        
</div>  
  
</body>  
</html> 
```


  
  



    
 
