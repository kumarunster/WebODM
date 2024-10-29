1) clone the project and switch to the branch:

```
git clone git@github.com:kumarunster/WebODM.git
cd WebODM
git checkout -b solar_panels
```


2) start the project with docker:

```

./webodm.sh start --dev

```

3) wait a while, after some time webodm is available under http://localhost:8000/

4) create first user/password on login (admin/admin)

5) on overview, import a project from this URL: https://nextcloud.raitsev.com/s/NL4NWsmNNfRJZsa/download/Kirchenrottweg-14102024-backup.zip

6) after import open the 3D Viewer. 3D Viewer should show the roof with some red measurements. On the Side Bar accordeon menu should be visible with "Solar Panels". Click on that Tool will create an Area Measure on the 3D Model.

7) Source code is located under: ./app/static/app/js/vendor/potree/build/potree
main files is potree.js, check as well my initial commit https://github.com/kumarunster/WebODM/commit/726c23b71e867c404ed41bde770f9fe7263a2aae for changes

### Target:
* Modify the Solar Panel Tool in the way, that we can create and place simple rectangles with fixed size (1,11m x 1,76m) on given surfaces.
* Fix the Remove All button, so that created solar panel objects are removed
* If above works, verify, if some texture on is possible on the rectangle.