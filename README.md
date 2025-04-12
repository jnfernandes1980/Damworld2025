# Damworld2025 - Using HEC-RAS for dam break simulation - Case Study

Welcome to this tutorial for the lecture on dam break simulation. 
It will guide you and cover the main steps to get the inundation due to a breach in a dam.
These are the main components:
![image](https://github.com/user-attachments/assets/470b280e-6676-489a-80e2-f6a7078227a4)

This is the current User Interface of HEC-RAS:
![image](https://github.com/user-attachments/assets/393f1d6a-71f0-46d7-aea4-75b10936c332)

Besides other functionalities, the most important sections are #Geometric data, #Simulations and #RAS Mapper

# STEP 0: Get terrain data

Download Elevation Data https://search.earthdata.nasa.gov/search

1. Register
2. Choose the area that is important for you
3. Download SRTM (1 sec arc in tif format)
  
   ![image](https://github.com/user-attachments/assets/9e5ddcee-ceae-4aff-b4bf-0868e8351ec0)

# STEP 1: Create terrain

1. In RAS Mapper - Add projection (https://spatialreference.org/)
2. Add new terrain with downloaded data (if you have more than one data set, order it. Put in the top the most relevant (LiDAR for the river and SRTM for the floodplains, for example) 
3. Create terrain
   
   ![image](https://github.com/user-attachments/assets/6e825357-2ded-46f2-885c-8c815e2af5c5)
Register

# STEP2:Create Storage Area (It will be your reservoir)

1. In RAS Mapper

2. Add new storage area

![image](https://github.com/user-attachments/assets/8ebd8ff7-8314-49b0-a84f-03ae3bd38780)
![image](https://github.com/user-attachments/assets/4eb3a4a1-1d37-4947-ab12-4c54ed3bdb58)


# STEP3:Create Connection storage area - 2d mesh (It will be the dam you want to breach)


![image](https://github.com/user-attachments/assets/1e67c8ef-2e0c-4df0-a355-baf680146113)

# STEP4: Create valley where breack wave will propagate (It will be affected area)
1d
![image](https://github.com/user-attachments/assets/f3722c68-7a9c-4b33-b480-58f61433c7bd)
![image](https://github.com/user-attachments/assets/799c0b21-5bb2-4d67-8775-a400ef2db6ad)
2d
![image](https://github.com/user-attachments/assets/3a210463-8c2f-4817-abc6-37e7c6c78803)

# STEP4: Run your model (Unsteady flow)

![image](https://github.com/user-attachments/assets/e1f8e35a-e9f2-4300-b847-5739405be56f)



![image](https://github.com/user-attachments/assets/6ee87f42-bf45-49fa-b8ec-52434e17298e)



## Disclamer: this repwas done for support the lecture on dam break flood simulation using HEC-RASfrom the Conference Damworld 2025 (LNEC - João Nuno Fernandes, jnfernandes_at_lnec.pt)
