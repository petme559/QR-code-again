# ARPymol - Augmented reality from Pymol

  Model preparation:
  - Load and customize your model in Pymol (2.4 or above!)
  - Avoid using mesh representation, and minimize sticks, balls and lines, as they will increase the file size. The size limit is 25 MB.
  - Transparency and labels will not be applied in the model, but measurements will be visible, only without numbers.
  - To generate your 3D object, use the command:' save filename.gltf ', or go to ' File - Export image - GLTF... '
 
  AR:
  1. Create a new repository in your GitHub profile
  2. Import this repository ( https://github.com/MokosDaniel/ARPymol )
  3. Upload your gltf model in your repository ('Add file' or just drag and drop it in the browser and commit changes)
  4. Edit the index.html file and change the name of the model "yellow.gltf" in line 16 to the name of your object, "filename.gltf"
  5. Commit changes, then in the repository, go to 'Settings - Pages - Branch' and select 'main' from the list
  6. Save, and after a few minutes the link for your AR scene should show up in the Settings - Pages site.
 
To View the AR scene, go to the URL shown in Pages on a device with a camera, and look at the marker image "3Dmarker.png".

Generating a QR code is a good idea for a way to share and access the URL (https://www.qrcode-monkey.com/)  
    -Make sure you use the URL found in Pages, not the URL of the github repository
 
 
In case you want to use a personalized Marker:
  - Generate and download the marker AND the image here: https://ar-js-org.github.io/AR.js/three.js/examples/marker-training/examples/generator.html
      - Use these tips: https://medium.com/chialab-open-source/10-tips-to-enhance-your-ar-js-app-8b44c6faffca
      - do not change the "pattern ratio"
  - Upload the .patt file to your repository
  - Change the 'url' of the marker in line 12 of index.html to the one you uploaded "markername.patt"
  - Once updated, the model should show up when looking at the image of your new marker.
 
Any changes you make usually take around a minute to take effect in the webapp.
If you have issues with the site zooming in, either turn off the override zoom function in your browser or press the fullscreen button.
