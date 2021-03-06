## Asset Details

This weblet provides a typical use-case of displaying a list of items and be able to modify, delete or get details about it in place.

The Asset Details weblet displays a list of Assets available in the system and allows you to  modify an Asset and display a quickinfo about it. It has filters to filter Assets based on _Installed Date_ and _Operational Status_.

#### View Components

* **Weblet** - display _Assets_ in the system

  ![Asset List Weblet](images/s1.PNG)

* **Dialog** - allows you to edit an Asset
  
  ![Asset Edit Dialog](images/s2.PNG)

* **Quick Info** - display additional details about an Asset

  ![Asset QuickInfo](images/s3.PNG)

#### Illustration

* Editing an Asset

  ![Asset Edit](images/s4.gif)

* Filtering Assets by Operational Status

  ![Filter by Op Status](images/s5.gif)

* Filtering Assets by Installed Date

  ![Filter by Installed Date](images/s6.gif)

#### Backend Components

* **SandboxBackend** - _Lucy model_ that provides data for the view to render with the following action sequences,
  * **ListAssets** - returns Assets in the system
  * **AssetDetails** - returns details about a single Asset
  * **UpdateAsset** - updates an Asset
* **Data Source**
  * **AssetDetails** - returns details about a single Asset
  * **ListAssets** - returns Assets in the system