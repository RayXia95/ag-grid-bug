# AgGridBug

## Steps to reproduce the bug using Ag-Grid Version 22.1.1

1. Open command prompt or powershell and clone this project
2. Change directory to the directory under ag-grid-bug (where the project was cloned to)
3. You need to have Node 10+, and npm version 6.4+ (Please install if you do not have those version. https://nodejs.org/en/download/)
4. Type and run: npm install
5. In order to perform the next step, you need to have angular cli downloaded. If you have angular cli downloaded and angular cli 8+, skip to step 7
6. npm install -g @angular/cli
7. Once finished wit the installation, type and run: ng serve
8. Open Google Chrome (or Microsoft Edge/Firefox) and type in the URL: localhost:4200
9. Verify that there is a grid with some data there (Toyota, Ford, Porsche)
10. Click and hold on one of the cell and drag your mouse to select a range of data
11. With data selected (attached screen shot), Hit Ctrl + c to copy the data (Windows machine)
12. Try pasting (ctrl + v) into a word document or notepad. Nothing shows up. This is the bug
13. Cancel the process ng serve 
14. Go into package.json and change the version of ag-grid-angular, ag-grid-community, amd ag-grid-enterprise to 21.2.2
15. Run: npm install
16. Run: ng serve
17. Repeat steps 8-12 (copy and paste works).
