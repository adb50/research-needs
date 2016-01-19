---
layout: rns
title: Standardized File Format for Traffic Count Files
interested-practitioners:
 - name: Andrew Rohne
   link: https://github.com/okiandrew
 - name: a name
   link: where can we find you on the internet
interested-researchers:
 - name: a name
   link: where can we find you on the internet
 - name: a name
   link: where can we find you on the internet
comments: true
---

# Description

This research would develop a standardized file format for traffic counting outputs.  

Currently, many of the traffic counting device vendors write to some state-based formats
which normally do not include 15-minute interval data by vehicle class, and frequently
are human-readable but not easily read by a computer. The differing datasets from the
traffic counter vendors has required agencies to either accept less-detailed data or
spend time writing code to translate poor formats to other formats just to get data to a
more usable format when that time could be better spent actually checking the count
itself of developing better procedures to screen traffic counts.  Additionally, traffic
counter equipment manufacturers appear to view their software (which is normally of low
quality) as the be-all-end-all and are apathetic to the needs of agencies to store counts
in a database that is open to other software (modeling software, GIS software, web
mapping software, etc.) and that it is fairly common for an agency to receive data from
multiple sources that use multiple different brands and models of traffic counting
equipment.

# Objective

A file format that can be rammed down the throat of traffic counting equipment vendors
that is basically a complete export of computer-readable data.  This format would be
open enough that it can include different data intervals (hourly, 15-minute, 5-minute,
per-vehicle) and data types (volume counts, class counts, speed counts, combined
speed/class counts).

# Benefits / Relevance / Priority / Urgency

The benefits of having one standardized format cannot be overstated, provided it doesn't
become like [this XKCD comic](https://xkcd.com/927/) mocking the situation of having multiple
competing standards.

Having one format makes it easy to share data.  A state DOT that takes counts can send one
file per count and expect that an MPO (or county, or city) can read the file without undue
effort (presuming the DOT creates the file correctly, which will hopefully be created
correctly by the traffic counter equipment software).  

Less time spent dealing with undocumented or poorly-documented file formats that require
software and a license to read means that the agencies looking at a count can spend more
time looking at the data as opposed to trying to figure how to look at the data.

The benefit to engineering consultants is a simple, standard deliverable that would
make it easy to provide traffic counts to their clients.

The benefits to all traffic count users is that one standardized format can make it
easier to visualize and store counts.  Similar to how GTFS has made it possible to
easily create tools to visualize transit lines (and even paved the way to a standard
transit model, STOPS), this would pave the way to the ability to have standard ways of
visualizing traffic counts.

# Suggested Funding

# Related Research

[Improving the Efficiency and Accuracy of the Oklahoma DOT Temporary Traffic Monitoring System](http://rip.trb.org/view/2015/P/1372619)

# Tasks

1. Fund this research
2. ...?
3. Profit!

# Implementation

Implementation would have to involve development contracts to traffic counting equipment manufacturers
like Diamond, Jamar, MetroCount, Peek, IRD, and probably others. With the format being computer-
readable and open, it would not be difficult for the community to develop and share tools to import
count data into a database or a travel model.
