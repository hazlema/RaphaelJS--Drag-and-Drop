Title:	Missing Drag and Drop functions in RaphaelJS
Author:	Matthew Hazlett

# Introduction #

RaphaelJS is an awsome library for doing canvas related projects in a cross browser fassion.

## This Project Contains ##

### Raphiel Extentions ###

What the extentions do is fill in a few little gaps in the library that specifically relate to drag and drop.  

### Class Library ###

A class that handles the Drag and Drop operations for you.  All you have to do is listen for the proper events.

#### Events ####

* Drag.fireEvent('dragStart', [this, this.intersectsWith(), dragAxis, dragInfo]);
* Drag.fireEvent('dragMove',  [this, this.intersectsWith(), dragAxis, dragInfo, dragValues]);
* Drag.fireEvent('dragDone',  [this, this.intersectsWith()]);
* Drag.fireEvent('dragOut',   [this, source]);

#### Functions ####
 
* Drag.add(orj); -or- Drag.add([obj, obj, obj]);
 
# Raphiel Extentions Information #

	 * Function: getFirst()
	 *     Args: none
	 *    Notes: This function walks the list of objects
	 *           in RaphaelJS the find the first object created
	 *  Returns: object
	 *      Use: firstObject = myObject.getFirst();
	
	 * Function: getAll()
	 *     Args: none
	 *    Notes: This function walks the list of objects
	 *           in RaphaelJS and returns an array of objects
	 *  Returns: [ object, object, object ]
	 *      Use: allObjects = myObject.getAll();
	
	 * Function: intersects(myObject)
	 *     Args: Object to compare
	 *    Notes: This function takes two objects and tells you
	 *           if they intersect
	 *  Returns: boolean
	 *      Use: isIntersect = myObject.intersects(myObject);
	
	 * Function: intersectsWith()
	 *     Args: none
	 *    Notes: This function looks at all the objects
	 *           and sees if this object intersects with any
	 *  Returns: [ object, object, object ]
	 *      Use: allIntersect = myObject.intersectsWith();

Please see the examples for more information.
