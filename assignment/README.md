# Assignment 06: Toward a final project and playing with D3

<!-- TOC -->

- [Assignment 06: Toward a final project and playing with D3](#assignment-06-toward-a-final-project-and-playing-with-d3)
    - [Part I: Finish lesson (4 pts)](#part-i-finish-lesson-4-pts)
    - [Part II. Your final project's topic, objectives, and data (3 pts)](#part-ii-your-final-projects-topic-objectives-and-data-3-pts)
        - [1. Data source](#1-data-source)
        - [2. Topic and geographic phenomena your map will explore](#2-topic-and-geographic-phenomena-your-map-will-explore)
        - [3. Map objectives and user needs](#3-map-objectives-and-user-needs)
    - [Part III. Making your own map with D3.js (3 pts)](#part-iii-making-your-own-map-with-d3js-3-pts)

<!-- /TOC -->

## Part I: Finish lesson (4 pts)

Work through the lesson and build the U.S. counties map using D3.js.

## Part II. Your final project's topic, objectives, and data (3 pts)

It's time to start thinking carefully about your final map project for MAP673. Using the process covered in Modules 04 &amp; 05, the deliverable for this week will include three pieces:

1. Your **data source** and (at least a sample of) the data required to meet the map's objectives.
2. The **map topic** and geographic phenomena your map will explore.
3. An articulation of the **map's objectives** and **user needs**.

Write thoughtful responses to the following questions within the markdown file named *topic-objectives.md* and commit to your map673-module-06-*username* repository.

### 1. Data source

This one is crucial. Sometimes we have high goals and ideas for a map. But if we can't easily and quickly get the data in a fast-paced class like this, we don't leave ourselves much time for the design and development phases. Demonstrate access to your data, or very minimally some ugly data that we can consider strategies for refining and cleaning up (though we recommend you begin the data wrangling immediately).

**Provide:** 
1. your anticipated data source and 
2. a small sample of the data (e.g., CSV/GeoJSON/Shapefile or a URL link to an accessible database). 
We need to be able to look at the data to give you quality feedback concerning your overall map objectives and what we can achieve in the next four weeks.

Still shopping for a topic? Consider looking through these open data resources for ideas and inspiration:

* https://data.world/
* https://www.data.gov/
* http://data.opengeoportal.org/
* http://www.naturalearthdata.com/downloads/
* https://www.census.gov/geo/maps-data/data/tiger-cart-boundary.html
* https://hub.arcgis.com/pages/open-data
* https://earthexplorer.usgs.gov/
* http://overpass-turbo.eu/
* https://download.geofabrik.de/
* http://sedac.ciesin.columbia.edu/
* http://www.opentopography.org/
* http://data.opengeoportal.org/
* http://krdc.uky.edu/data-products
* https://www.davidrumsey.com/


Reach out for help ASAP! Let us know what you're looking at or ask your course team members for advice on Slack or a Canvas discussion post. Most importantly, think about data and a map that you'll have fun making and that you'll be eager to share with those who are important to you.

### 2. Topic and geographic phenomena your map will explore

What are you mapping? Briefly describe the topic and the geography the map intends to represent. Also, provide a tentative title (and possibly a subtitle) for your project. Remember that good titles, while being provocative and potentially fun, can quickly summarize the mapping project. In more detail than the previous module, provide four aspects of your project.

**Provide:**

1. *What?*
2. *Where?*
3. *When?*
4. What is the tentative title of your project?

### 3. Map objectives and user needs

* Answer the question, "Why does the map need to be made?" Consider your position to the mapping project. If your design is to bridge a purpose with a format (in this case a web map), why are you the one to be designing it?
* Create a brief user persona and tell us why this person is using your map. How would you characterize them in terms of their expertise and motivation (i.e., novice/public, average, expert/domain-specific). Give them a name and tell us how (and why) they would use your map, e.g., in the field checking trail locations or on a desktop looking through economic statistics. 
* Imagine a scenario. It need not cover all potential use cases, but it should describe some possible actions users may take to meet their objectives (i.e., filtering the data, searching for an address, changing the attribute with a drop-down menu). Use Roth's interaction operators (Module 04/05) to describe these human-computer interactions (HCIs) better.

Provide wireframes or mockups if it helps your thinking at this stage. Again, write this using Markdown in the file named _topic-objectives.md_.

## Part III. Making your own map with D3.js (3 pts)

Either begin by building an HTML template of your own or copying and modifying the _index.html_ file from the lesson. Build your map within a file named _index.html_ within the _assignment/_ directory.

Choose two or more datasets of **polygon** features of anywhere in the world, at any scale. Obtain a GeoJSON representation of these data, and be sure they are unprojected WGS 84 latitude and longitude values. Then create TopoJSON versions of these GeoJSON datasets and include them within the _assignment/data/_ directory. Also, update the _meta.md_ file with the data source information and your process for simplifying/converting.

[Mapshaper](https://mapshaper.org/) be useful for quickly converting Shapefiles to GeoJSON and TopoJSON.

**Warning:** Be mindful of your file sizes and **do not commit files larger than 100MB to your Git repository**. GitHub will reject these pushes to the repository and create a headache.

An easy data source for experimenting with D3 is [geojson.xyz](http://geojson.xyz/), but feel free to use any data source. Note that we have not covered point features or making a thematic map (which we'll do in Lesson 07).

Modify the code examples from the lesson to center your geometries within the map. Style your geometries appropriately. The goal is to explore how to build a map with D3.js and feel free to experiment.

Also, try modifying the Bootstrap template and theme (such as by swapping in a new theme from [BootstrapCDN](https://www.bootstrapcdn.com/bootswatch/)).

Commit changes to your work using Git as you work, and push to the remote repository for backup, help, and the final submission.