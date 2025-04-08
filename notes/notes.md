# Notes

## Groups

- Groups - collecition of related functionality 
- Versions 
- Kinds - API types (objects). Each new kind version must keep all of the data from the pervious version
	- Example: `pod`, `deployment`, ...
	- A `kind` is meant to be backwards compatable
- Resources - refers to the kind in the api. While it may be 1:1 like Pod and `pods` it does not have to be.
- Scheme - Maps go type to the `GVK` (Group Version Kind)


## Go Code

- Spec & Status (in the types under `/api`)
	- K8s tries to make the state of the object equal to the `spec`. The result is written into a `status` object