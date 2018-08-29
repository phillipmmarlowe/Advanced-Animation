# JavaSsript Vectors: Lab 829#

###Objectives###
 - Create a vector object with properties and methods a Vector class
 - Understand Vector magnitude and direction 
 - Understand Vector addition, subtraction
 - Create getters and setters for magnitude and direction 


##Part I: Add a Vector constructor function to your lab ##
 - Get the Student_Labs repo from GitHub and 
 - Add an object factory function according to the pattern below


###Part II: Four JS Patterns for creating objects###

 -  Add the following code to your project (Do **NOT** copy and paste):
 

			//  JavaScript object patterns
			//  One:Ball Factory:: Build and return a Ball
			function ballFactory(rad){
			  var Ball = {
			    radius:rad,
			    getDiameter:function(){
			      return 2*rad;
			    }
			  }
			  return Ball;
			}

			// Two:Constructor function:: Simplifies the code above
			function Ball(rad){
			  this.radius = rad;
			   this.getDiameter = function(){
			     return this.rad*2;
			   }
			}
			
			//  Three:Add a method to the prototype
			Ball.prototype.getArea = function () {
			  return this.radius*this.radius*Math.PI;
			};
			
			// Four:Classical syntax::Hand holding for Java programmers 
			// Where does the function "getDiameter()" end up?   
			class ClassyBall{
			   constructor(rad){
			     this.rad = rad;
			   }

			   getDiameter(){
			     return this.rad*2;
			   }
			
			}


 -  Use the console to see where the methods are added to your object:
 
###Part III: Canvas Code###

 -  Study the code that creates a canvas and a context.  Use the patterns above to create four balls and animate each:





----


