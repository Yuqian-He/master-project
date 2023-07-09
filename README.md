# A Cross-Platform USD-based Rigging Schema for Streamlined Animation Workflow
## master project workflow
![4971688925138_ pic_hd](https://github.com/Yuqian-He/master-project/assets/104955148/036f4db0-a106-4304-9a35-c47ecffd5d6c)
## aims
mesh, skeleton, bind, weight (deformation of mesh)
![4981688926069_ pic](https://github.com/Yuqian-He/master-project/assets/104955148/4f32c3c1-24a5-4329-a1a1-85c50fa41070)
![4991688926177_ pic](https://github.com/Yuqian-He/master-project/assets/104955148/6ba5dc8a-ab23-42d4-9bbd-10963835a839)
## MAYA
maya translator (mesh):
Create c++ project which can access maya API and USD API ---> generates .bundle file (package related resources, libraries) ---> maya plugin.
https://github.com/Yuqian-He/master-project/assets/104955148/9d8fe5b5-7f06-4188-8237-92f830a4fb9d
https://github.com/Yuqian-He/master-project/assets/104955148/6f4e9e5c-154a-4f6c-9930-c4f2ce078fd2

## HOUDINI
houdini translator (mesh):
Create c++ project which can access HDK and USD API ---> generates SOP.dylib file ---> houdini SOP
Don't require mesh with all quad faces or triangle faces.
https://github.com/Yuqian-He/master-project/assets/104955148/599517f3-4f94-4351-8b65-101b70dbb0cf

## =======================================================
This is the all workflow transfer from maya to houdini, but just transfer mesh.
## USD
skeleton ---- non-concrete IsA Schema (translate, rotate, bind)
bind ---- API Schema (bindPose, bindMatrix)
weight ---- abstract API Schema (weightSize, werightList)

test creating a new USD schema (failed) 








