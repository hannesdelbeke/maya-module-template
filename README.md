# maya-plugin-template
- click 🟩`use this template` to create your GitHub repo, & clone it
- rename the `MyModule` folder & `MyModule/myModule.mod` 
- open the `.mod` file and change the module name inside
- replace this README.md with your own instructions
- Add a LICENSE

### Module
- the MyModule directory contains the module files.
- the icons, plug-ins, presets, and scripts subdirectories are the default directories that Maya expects to find in a module. You can choose to use different directories or multiple directories in your module, but you will need to specify these in the (.mod) module description file.
  - Add any icons used in your add-on to the icons directory
  - Add C++ and Python plug-ins to the plug-ins directory
  - Add presets to the presets directory
  - Add any MEL or Python scripts to the scripts directory
- Create a module description file file with the `.mod` extension (see [docs](https://help.autodesk.com/view/MAYAUL/2023/ENU/?guid=Maya_SDK_Distributing_Maya_Plug_ins_DistributingUsingModules_ModuleDescriptionFiles_html))

### plugin
Plugins let the user easily enable / disable a tool in Maya.  
They also let you run code on startup, without editing the `userSetup.py` file, keeping your Maya clean / vanilla.  
![](https://www.sidefx.com/media/uploads/products/engine/hengine_maya_load.jpg)  
This project includes a sample `helloWorld.py` plugin - A plugin sample from the Maya docs. 
plugins should be placed in the `MyModule/plug-ins` folder

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
