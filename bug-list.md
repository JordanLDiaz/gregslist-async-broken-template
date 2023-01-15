# Bug List

Car Model File
1. Changed name="price' to name="mileage" on the form so you can check the network tab and see that it is a required path 
2. In the list template I took out the string interpolation for make on model and put Honda Civic.
3. In constructor in the Car Model I changed data.price || 0 to 500 that way every car is changed to 500 after it is created. When it gets pushed into the model

Service File
1. Took off the cars on the endpoint that is getting all my cars so it is immediately throws a 404
2. Took off the await on the createCar function when calling to the api
3. In create a car I also changed the body name in the parameters compared to one that I am using to send up to the api
4. In removeCar I took out the id in the parameters and also when I send it up to the api

Controller File
1. On appState.on in the constructor I changed 'cars' to 'cart' in drawCars that way listener doesn't match the name in the appState and to show off what that means.
2. Took off the word async in front of the editCar function
3. Took off the await in Pop confirm so it fires immediately.