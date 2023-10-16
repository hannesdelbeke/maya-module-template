# Maya Python plugin template

A template to quickly make a Python plugin & module for Maya

### Instructions
- click 🟩`use this template` to create your GitHub repo, & clone it
- Module setup 
  - rename the `MyModule` folder & `MyModule/myModule.mod` 
  - open the `.mod` file and change the module name inside
- Plugin setup
  - rename the demo plugin `MyModule/plug-ins/hello_world.py` 
  - add load & unload code to the `initializePlugin` & `uninitializePlugin` methods
  - optionally handle command registration on load & unload 
- add your Python modules to `MyModule/scripts`
- Optional
  - replace this `README.md` with your own instructions
  - Add a LICENSE
  - delete all `.gitkeep` files

### Module

A module let's you change the Maya environment, without changing your Maya installation.  
e.g. add resources, plugins, environment paths, ...  
We use this to register our plugin with Maya in a modular way: When the user registers the module, everything else is automatically hooked up.  

- the MyModule directory contains the module files.
- the icons, plug-ins, presets, and scripts subdirectories are the default directories that Maya expects to find in a module. You can choose to use different directories or multiple directories in your module, but you will need to specify these in the (.mod) module description file.
  - Add any icons used in your add-on to the icons directory
  - Add C++ and Python plug-ins to the plug-ins directory
  - Add presets to the presets directory
  - Add any MEL or Python scripts to the scripts directory
- Create a module description file file with the `.mod` extension (see [docs](https://help.autodesk.com/view/MAYAUL/2023/ENU/?guid=Maya_SDK_Distributing_Maya_Plug_ins_DistributingUsingModules_ModuleDescriptionFiles_html))

### plugin
Plugins let the user easily enable / disable a tool in Maya (with Maya's plugin manager)  
They also let you run code on startup, without editing the `userSetup.py` file, keeping your Maya clean / vanilla.  

![](https://www.sidefx.com/media/uploads/products/engine/hengine_maya_load.jpg)  
This project includes a `helloWorld.py` plugin (a demo plugin from the Maya docs).  
Plugins should be placed in the `MyModule/plug-ins` folder

### scripts
Your Python modules should go under `myModule/scripts`.  
It might be a good practice to develop them in a separate repo, so the module can have it's own `pyproject.toml` & `requirements.txt`

### icons
TODO how to access icons in script

### presets
attribute presets
- [ ] TODO createa a sample  
[docs](https://help.autodesk.com/view/MAYAUL/2023/ENU/?guid=GUID-B90EF3C9-EFB8-4BBC-B9A5-69F7EC86B3C3)

### installation
TODO
### menu entry
TODO
### tool entry
TODO
### shelf entry
TODO
### references
- [module layout docs](https://help.autodesk.com/view/MAYAUL/2023/ENU/?guid=Maya_SDK_Distributing_Maya_Plug_ins_DistributingUsingModules_CreatingAModulePackage_html)
- [module install docs](https://help.autodesk.com/view/MAYAUL/2023/ENU/?guid=Maya_SDK_Distributing_Maya_Plug_ins_DistributingUsingModules_InstallingModules_html)
  - you can manually install the module by moving the MyModule folder in the maya modules folder 
  - maya searches for modules in the `MAYA_MODULE_PATH` env var
  - you can also add paths to `Maya.env` file
- [maya plugin docs](https://help.autodesk.com/view/MAYAUL/2024/ENU/?guid=Maya_SDK_A_First_Plugin_Python_html)


plugin from 
