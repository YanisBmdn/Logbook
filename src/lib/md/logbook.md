# LogBook

For the next 6 months, I'll be logging my advancements every day in this logbook.  
Its content may be utterly random, but its goal is for me to have a record of my research and for anyone to have an insight into what I am working on and any interesting findings I may come upon. Although for now very basic, this logbook will evolve throughout my stay to someday look more decent.

~~My subject revolves around finding a way to combine multi-source satellite imagery to provide an accurate way to classify tree-specific species (whether in urban areas or high-density forests).~~

**My current subject is : Conversational Agent Fact-Based Environmental Discussion based on Data Visualization"**

## Thu. 11-07-2024

Today's goals are :

- &#9745; Define the metrics / visualization that will be used.
- &#9745; Further define MVP and how the system will work

Found out about [Copernicus Data Space Ecosystem](https://dataspace.copernicus.eu/) which holds all open data provided by Copernicus and ESA (European Space Agency)

- I will definitely use Sentinel-2 data for vegetation related metrics (NDVI, EVI)
- A data source for air pollution is also needed - [Sentinel-5P](https://sentinels.copernicus.eu/web/sentinel/copernicus/sentinel-5p) data could prove useful and is, as per ChatGPT, the "Best source for high-resolution atmospheric pollution mapping at a global scale"
- Another data source for surface temperature could be Landsat 8 / 9 coupled with ground-truth data of local weather stations.

I have also thought more about how the system will work. I have yet to define the task delegated to the LLM.

However, one thing I want to be careful of is using LLM only when it is necessary and purposeful, and where it cannot be replaced by another more efficient and simpler system. The aim of this is to reduce as much as possible the impact of the research and application on its environment.
I truly want to provide a lightweight, sustainable solution. **Temperance is the key**.

## Wed. 11-06-2024

Defined a schedule, and use cases for the research.
Main use cases will be :

- Education & Information
- Urban planning support
- Research tool

Questions that could be asked to the agent could be :

- “How has vegetation coverage changed in Nagoya Atsuta-ku over the last 10 years?”
- "What local environmental examples can I use to teach about climate change?"
- "Which neighborhoods have the lowest tree coverage and highest summer temperatures?"
- "Generate time series analysis of vegetation health in Aichi prefecture protected area"

Also had a weekly seminar, where my supervisor suggested to use audio based interface. I originally intended to have a chat based interface, but this
could be very interesting ! I could provide in parallel a web, conversational interface for a broader use. But I think I'll stick with the audio one
for the moment.

## Tues. 11-05-2024

After a lot of searches and a meeting with supervisors I decided to slightly shift my theme. Training a model is quite complicated,
could take time and I think it's not fit to a 6 month research plan. This change was suggested by my supervisor and I'll go with it ! Thus, my new theme is :

> **Conversational Agent Fact-Based Environmental Discussion based on Data Visualization**

This research project aims to create a conversational LLM based agent that provides information on environmental policies and urban planning decisions while also integrating relevant data visualizations to enhance understanding and facilitate fact-based discussions.

The topic change doesn't make my prior searches and documentation obsolete, as I'll probably use satellite imagery nonetheless !!

## Wed. 10-30-2024

- &#9745; Prepare seminar + weekly report
- &#9744; Define which data sources will be used

## Tue. 10-29-2024

- &#9745; Define clearly what my research covers (what will I do / I won't do)
- &#9744; Start saving ground-truth data for model training

I have actually been searching for good **spatial resolution** LIDAR / SAR imagery, to get the elevation of tree canopy for segmentation. I have found [one project](https://gee-community-catalog.org/projects/meta_trees/#dataset-citation) but it's on a singular point in time, so I must consider using this kind of data or not.

I haven't talked about what **spatial resolution** is, so let me showcase it with an example :

- Google maps basically has some very good spatial resolution here we probably something close to **20cm per pixel** (depends on where you look, has it creates a mosaic of many different imageries)
  ![Google maps satellite imagery](/images/1029-satellite1.webp)

- Sentinel has lower resolution, for its RGB bands at **10m per pixel**
  ![Sentinel 2 RGB satellite imagery](/images/1029-satellite2.webp)

## Mon. 10-28-2024

- &#9745; Setup a schedule for the next 6 months
- &#9745; Redefine my subject based on last Thursday's feedback
- &#9744; Concretly define ground-truth data

Defined my schedule for the next 5 months (1 month has already passed...). Waiting for my supervisor feedback on it.
![Schedule](/images/1028-Schedule.webp)

Meanwhile, I tried redefining my subject more to lean towards Civic Tech. I have multiple ideas of outcomes for the research but it's very hard to define a limit. For the moment, I want to build my own AI Model on different data sources (multispectral, RGB). I have found [Canopy height data](https://langnico.github.io/globalcanopyheight/) but the fact that there is only a single point in time makes it hard to utilize it for tree evolution...

I have thought about leveraging LLMs (RAG + Function calling) as an interface for the data of this research. On top of probable open-data !

## Thu. 10-24-2024

Had a meeting that further extended the reach of my project. As the lab I am currently working in mainly revolves around [Civic Tech](https://en.wikipedia.org/wiki/Civic_technology). One of my supervisor suggested that I could use the data of my research to provide fact-based checking for public debate / deliberation. This could prove very interesting !!

I'll look deeper into it. I think time as come to set a schedule up.

## Wed. 10-23-2024

Found a gold mine for ground-truth forest dataset. This will be of immense help and also will make me consider new possibilites.
[Awesome forests](https://github.com/blutjens/awesome-forests?tab=readme-ov-file)

Also gave the presentation, which went pretty smootly ! I relied a lot on my script for the japanese part but I am still pretty proud. One of my colleague also gave me information about datasets provided as open-data by the government of Japan. I should look into it.

- [Geospatial data](https://www.geospatial.jp/ckan/organization/rinya)
- [Forest open data](https://nlftp.mlit.go.jp/ksj/gml/datalist/KsjTmplt-A45.html)

## Tue. 10-22-2024

I have to give a presentation tomorrow about me and my research theme. I decided to give myself a challenge and do the self-introduction in Japanese (help). The script of the self-introduction is all written, but it's meant to just be an emergency backup. I'll try to use it as little as possible.

In the meantime, I have further explored QGIS possibilities and tried to understand how the software works.

## Mon. 10-21-2024

I have been searching for ground-truth data as per my advisor's feedback.  
I have stumbled upon a few datasets:

- Planted
- Pureforest
- TreeSatAI

I have also been exploring with QGIS, an open-source Geographic Information System (GIS).
Here's a sample of TreeSatAI dataset.

![QGIS1](/images/1021-QGIS1.webp)

![QGIS1](/images/1021-QGIS2.webp)
(Yeah I know, it's a mess...)

## Sun. 10-20-2024

I have finally settled on a subject after 2 weeks of searching. Today, I just got this website running with very minimal content and styling. The logging will debut tomorrow!  
As for now, here's just a simple website I stumbled upon which has pretty impressive photography: [ESA Earth from space](<https://www.esa.int/ESA_Multimedia/Sets/Earth_from_Space_image_collection/(result_type)/images>).
