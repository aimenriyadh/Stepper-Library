# Stepper-Library

## Screenshots
![Image Result](https://scontent.fgza6-1.fna.fbcdn.net/v/t1.0-9/106503813_693000678211700_2733733955416928403_n.jpg?_nc_cat=102&_nc_sid=07e735&_nc_ohc=4NiB_Ur8XbAAX9iQAH0&_nc_ht=scontent.fgza6-1.fna&oh=9c30aefb155035a8e040691afc145f9c&oe=5F22F65B)
## How Add Library To Your Project
##### in `build.gradle` on Project Level you should add 
##### `maven { url 'https://jitpack.io' }` in 
`allprojects { 
     repositories { 
        maven { url 'https://jitpack.io' }
      }
 }   
   `
##### After Thet add `implementation 'com.github.kareemradwan:Stepper-Library:0.1'` in `build.gradle` in App Level
##### in `dependencies` Tag


## How Library Work

##### We Need Create Step Class for Example `Order` and `OrderAdapter` 
##### The Class `Order` Must Be Implements Interface `IStep` and Implementaion Require Method `isChecked()`
##### The Class `OrderAdapter` must be inherited class `StepAdapter` with Generic Type `Order`
##### The Class `OrderAdapter` Require List of Any Class Implements Interface `IStep` in Our Example `Order`

`
StepAdapter<Order>(list)
`

##### In `OrderAdapter` We Should Override `onCreateView` Method 
##### The Method `onCreateView` take a Model of `Order` and Sould be Return `View`

##### After Adapter Ready You Can Assign Adapter For `SteeperView` 

##### You can Register The Activity as Controller to Notifiy When `SteeoerView` Finish ( in Last Step )



## What is Next:
##### - The Developer Can Custmise Color of Step
##### - Add Animation for `CheckBox` When be Selected


## About Developer:
##### Name: Kareem E Radwan
##### Email: kareem.e.radwan@gmail.com

