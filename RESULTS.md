
1. vehicles with different levels of visibility

pcl_screenshots folder contains 3 screenshots.
* screenshot(3.0) contains different examples of incoming and oncoming vehicles:
    - Only part of the closest vehicle is visible
    - Some of oncoming vehicles are partly hidden by another oncoming vehicles
    - Oncoming vehicles are located on different lines
    - vehicle with trailer
* screenshot(3,199) contains turning cars
* screenshot(3,100) contains truck

recognizable features:
* vehicles have similar height(except trucks)
* car windows are visible on PCL images
* wheels are visible on PCL images

2. models performance

performance folder contains screenshot with performance for both models and each datafile(sequence).

1. Darknet model shows much better results for the first data file: precision ~0.9 recall ~ 0.75 vs precision ~0.7 recall ~ 0.5
2. Both model show similar detection precision for second data file: ~0.4 however detection recall is better for darknet: ~0.6 vs ~0.4
3. Darknet model shows better results for the third data file too: precision ~0.8 recall ~ 0.6 vs precision ~0.55 recall ~ 0.35
