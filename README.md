# UOCIS322 - Project 4 #
You'll learn how to write test cases and test your code, along with more JQuery.

## Overview

This app is a RUSA ACP controle time calculator, built with Flask and AJAX.
> That's *"controle"* with an *e*, because it's French, although "control" is also accepted. Controls are points where a rider must obtain proof of passage, and control[e] times are the minimum and maximum times by which the rider must arrive at the location.

### ACP controle times algorithm

The algorithm for calculating controle times is described here [https://rusa.org/pages/acp-brevet-control-times-calculator](https://rusa.org/pages/acp-brevet-control-times-calculator). Additional background information is given here [https://rusa.org/pages/rulesForRiders](https://rusa.org/pages/rulesForRiders).

I have essentially replaced the calculator here [https://rusa.org/octime_acp.html](https://rusa.org/octime_acp.html).

## How to Use

### Building and Serving

Build the docker image by running `docker build -t <image_name> .` from the `brevets` directory.

Serve the image in a container by running `docker run -d -p 5000:5000 <image_name>`.

### Using the App

Once the container is running, you can access the app via a web browser by navigating to `localhost:5000`.

You can then set the brevet length and start date/time with the input boxes at the top of the page.

Once the brevet length and start are specified, simply fill in the desired distances for each checkpoint in either miles or km. The webpage will automatically populate checkpoint open and close times.

## Authors

Michal Young, Ram Durairajan. Updated by Ali Hassani. Updated again by Zack Johnson :)
