#**Lapter.js**
======
##**Javascript adapter to work with localStorage**

###**API:**

**namespace()**

	 default: 'lapter' - namespace for single application - 
     just propery in localStorage
     will contain singleton object to storage data of one applicaton
	`Lapter.namespace('my_storage');`
    

**setId()**

	Set time or session_id mark to current localStorage Lapter in given namespace
    `Lapter.setId(3);`


**getId()**

	Get uniq id for Lapter in given Lapter namespace. 
    May be usefull to destroy previous Lapter
    `Lapter.getId()`
    

**add()**

	Add javasctipt object to Lapter object (Backbone model as json for example)
	`Lapter.add('test_model');`
    

**set()**

	Set new data to existing Lapter property (rewrite)
	`Lapter.set('test_model',{data:[1,2,3,4,5]});`
    

**get()**

	Get object from Lapter
    `Lapter.get('test_model');`
    

**clear()**

	Erase data from property in localStorage
	Lapter.clear('test_model');
    

**remove**

	Delete property from Lapter
    `Lapter.remove('test_model');`
    

 **hardReset()**

 	Delete Lapter namespace and all data from localStorage
 	Lapter.hardReset();        