# License-OCR

I am an OLD SCHOOL NERD

Clone/Download

And since Git doesn't allow file size bigger than 100MB, download the sample.mpy video from the repo link sent or at this link - https://www.pexels.com/video/traffic-flow-in-the-highway-2103099/
This is the Video which the entire code, seperates it into image frames, which util.py file goes ahead and analyzes and finally generates a test.csv with all number plates identified.

The add_missing_data.py file assigns a numeric score, and generates a test_interpolated.csv

The visualize.py file is cool, it takes that test_interpolated.csv and the sample.mp4 and voila adds a text label in the output video which shows the Number Plate of the vehicles, the output file generated is out.mp4, and visualize.py makes use of mp4v codec to do that.

If Collab automatically downloads all libs then no need of pip install -r requirements.txt

Step 1 - 
Run main.py - it generates the test.csv (make sure sample.mpy exists in the root dir)
Cmd - python main.py

Step 2 -
Run add_missing_data.py
Cmd - python add_missing_data.py
In the repo shared, it had this mentioned "Run the add_missing_data.py file for interpolation of values to match up for the missing frames and smooth output" as the reason, need to get some more info on this part but it's needed.

Step 3 (Final Step) -
Run visualize.py this might take a while 10-15 mins depending on hardware config, this generates the final out.mp4 which has Number Plate shown for the vehicles in the video sample.mp4

Cmd - python visualize.py
