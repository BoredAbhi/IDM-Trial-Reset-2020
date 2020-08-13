# IDM Trial Reset 2020
### Reset IDM trial without any external softwares (working in 2020).

I found this solution in [J2TEAM/idm-trial-reset](https://github.com/J2TEAM/idm-trial-reset/)'s Issues section [here](https://github.com/J2TEAM/idm-trial-reset/issues/10#issuecomment-616135590). Making this repository for wider reach. 
### Steps to fix IDM trial :
1. Search ``` run ``` in windows search and open the app.
2. Search ``` regedit ``` and open the app.
3. Navigate to : ``` HKEY_USERS\S-1-5-21-2092034274-3617384386-2923495293-1001_Classes\WOW6432Node\CLSID\{1890893f-6284-4de7-a5e3-46beb213ce98} ``` 

  **Note:** "_S-1-5-21-2092034274-3617384386-2923495293-1001_Classes_" will change for every system but it will always end in "_Classes".

4. Delete this key and IDM should start working as before.

### Another approch for automating this work:
1. Note the "_S-1-5-21-2092034274-3617384386-2923495293-1001_Classes_" value for your system.
2. Edit the ``` reg ``` file in this repo in Notepad and add your key.
3. Run the ``` reg ``` file and it will automatically delete the IDM entry.
4. Enjoy 
