# Mapping Youth Population Distribution Across California Counties

## Why I Made This
I'm interested in urban planning and environmental studies, and one thing that stuck with me is how much a simple statistic like "percentage of people in their 20s" can say about a place — whether it has enough housing for young workers, whether transit reaches them, whether jobs are actually there. So for this project I used ArcGIS Pro to map that percentage across every county in California and see what patterns showed up.

## What I Did
**Getting the Data**
I started with the `CountiesAgeY` layer, which joins census data with county boundaries, from the Chapter 4 geodatabase (`github-lee.gdb`).

**Making the Map Readable**
I used Graduated Colors symbology with Natural Breaks (Jenks) classification, split into 4 classes based on the percentage of people in their 20s. I also reversed the color order so darker shades mean a higher percentage, which just felt more intuitive to read at a glance.

**Layout**
I labeled populated places at 8 pt so you can still tell where you're looking without cluttering the map, then built a portrait layout with a title, north arrow, and a legend I trimmed down so it only shows what actually matters.

## What I Found
The counties with the highest percentage of residents in their 20s weren't the biggest cities — they were college towns: Yolo County (14.7%, UC Davis), Butte County (10.6%, Chico State), Santa Barbara County (10.3%, UCSB), San Luis Obispo County (9.7%, Cal Poly SLO), and Santa Cruz County (9.3%, UC Santa Cruz). Seeing that pattern show up so clearly on the map made it click for me in a way just reading a spreadsheet wouldn't have. The lowest percentages were in counties like Marin, El Dorado, Mendocino, Lake, and Nevada — places that tend to skew older and more rural. It made me think about how useful a map like this could actually be for planning: a county with a young, renter-heavy population needs a different housing and transit strategy than one with an older, more settled population.

## Files
- Project package: `Github-Lee-Youth2.ppkx`
- Submitted as: `Github-Lee-Youth2.ppkx.z
- source was https://data.census.gov/
