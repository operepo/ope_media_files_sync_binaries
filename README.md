# Install Canvas Files
This contains instructions on installing the courses into your canvas environment and getting media files working in your local copy of the SMC tool.

## Error Syncing Media Files (api-ms-win-crt-runtime-i1-1-0.dll)
You will need the visual studio c++ 2015 runtime files installed on your system to run this tool. It is included in the zip file as well as at the microsoft website.
- vc_redist.x86_16_19.exe - This will install the VS C++ Runtimes for 2015 through 2019


## Canvas Install
- Create a new courses in Canvas
- In the course, go to "Settings -> Import Course Content" and choose "Canvas Course Export Package" and select the correct IMSCC file

## SMC / Media Files Install
- Run the push_media_files.bat tool to copy the movies and google docs files into the SMC tool at your facility. Follow the prompts (NOTE: User/Password are your standard user/password used for the OPE SyncApp)

## SMC / Media Files - PULL
- You can pull media files from an SMC server by running the pull_media_files.bat file. You can put in a search term and it will search movies and document categories and tags for this term and download them all to the local folder. This is how you pull media FROM the SMC so that you can take it inside the facility.

## Change URL (OPTIONAL - Do this ONLY when NOT using https://canvas.ed)
Do this ONLY if you use a differnt URL for the canvas and SMC server (Things are already setup for https://smc.ed and https://canvas.ed)
- Go to the SMC tool
- In the menu, find "Media -> Offline Conversion -> Find/Replace (mass edit course)"
- Select the course
- Choose "Custom Find/Replace"
- Enter your pattern to find in the left side
  * To replace https://smc.ed - put smc.ed with out the https://
- Enter your pattern to replace with in the left side
  * Put in your new domain name - e.g. if your smc is at https://smc.correctionsed.com, then put smc.correctionsed.com
- NOTE: You can try it without writing changes to see how well it works! Then run it again if it looks good with the write changes box checked
- Once you are done - pick the "(Choose a differnt course)" link towards the top and repeat with each course

## DONE - Your courses should work in an offline environment.

