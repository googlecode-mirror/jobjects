jObjects is a Framework that let you create PHP objects in JavaScript and use them like if you where in PHP enviroment.

## Example ##
```
// Set the URL where the calls will be made
jObject.options.url = 'index.php';

// Create a new instance of your class, called Perro in this example
// and send the parameters in an array.
var rocky = jObject('Perro', ['Rocky', 'Bulldog']);

// Change the value of a variable in your instance
rocky.val('nombre', 'Jorge');

// Call a method with no results, and send parameters in an array
rocky.call('setRandomEdad', [4, 12]);

// Call a method with results
var nombreYRaza = rocky.call('getNombreYRaza');

// Get the value of a variable
var edad = rocky.val('edad');

alert( nombreYRaza + '\nEdad: ' + edad );

// Destroy all data
rocky.die();
```

## Downloads ##
  * 2008.01.29 [jObjects.v0.4.rar](http://jobjects.googlecode.com/files/jObjects.v0.4.rar)
  * 2007.11.22 [jObjects.v0.3.zip](http://jobjects.googlecode.com/files/jObjects.v0.3.zip)