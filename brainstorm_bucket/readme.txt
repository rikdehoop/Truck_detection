**in this txt file you can write anything you might want to talk about later or put away as an conceptual idea**
________________________________________________________________________________________________________________


BGT got parkeerspots in the wegdeel dataset, can be filtered out but maybe not complete in private areas

To prevent al containers to be detected even if there is no truck atached to it, we can choose to only train on the truck and not the atached container, altough this might give other unexpected issues, worth a discussion..

In post processing use lenght of object as filter-criteria to filter out the fans and smaller mis-detected vehicles












_________________________________________________________________________________________________________________
**POC POSSIBLE WORKFLOWS:**

**| POC WORKFLOW if no open data is compatible
__________________________________________________________
1. GO TO https://www.beeldmateriaal.nl/data-room and use the data portal with the ibis tereinen dataset (see vector_data) to donwload ortho mosaic imagery (instruction video: https://www.beeldmateriaal.nl/data-room).
2. Cut the imagery in even sizes of 640 that are compatible with yolov8, use the following python script for this (chop.py)
____
Once dicided which part of the truck needs to be trained based on logic to get the best outcome START MANUAL ANNOTATION PROCES USING LABELIMG
3. Use labelIMG to label al trucks
4. after labeling 2000 images split the data in training en validation datasets, spit balance should be 70/30
5. Start training the model
6  Test results
7  rapport results, reflect on results 
8. apply post processing methods to imporve final results
9  rapport results, reflect on resulst
10. conclude if good enouge or model needs adjusting




**| POC WORKFLOW if open data is compatible
__________________________________________________________
5. Start training the model
6  Test results
7  rapport results, reflect on results 
8. apply post processing methods to imporve final results
9  rapport results, reflect on resulst
10. conclude if good enouge or model needs adjusting

