# Final-Project-Snippets

A collection of code snippets to help with your final project!

*Note: Some datasets in WPRDC have different names for the various neighborhoods. These snippets use the dataset from the "Data-Visualization" lab.*

### Installation
---
1. Either clone this project or download it as a ZIP
2. Copy the `fpsnippets.py` and `ZIP_TRACT_032020.csv` to your final project folder.
3. Import the helper methods using `import fpsnippets`

### Methods
---
#### `fpsnippets.geo_to_neighborhood(latitude, longitude)`
* Arguments: 
    * `latitude`: float
    * `longitude`: float
* Returns: (string) The name of the neighborhood that contains this point or `None` if the point in not in a neighborhood.

#### `fpsnippets.zip_to_neighborhoods(zip_code)`
* Arguments: 
    * `zip_code`: integer
* Returns: (list of strings) A list of neighborhoods within this zip code.

#### `fpsnippets.census_to_neighborhoods(census_tract)`
* Arguments:
    * `census_tract`: integer
* Returns: (list of strings) A list of neighborhoods in this census tract.


### Usage
---
```python
>>> fpsnippets.geo_to_neighborhood(40.440624, -79.995888)
'Central Business District'

>>> fpsnippets.zip_to_neighborhoods(15282)
['Bluff', 'Central Business District']

>>> fpsnippets.census_to_neighborhoods(42003070900)
['Squirrel Hill North', 'Bedford Dwellings', 'North Oakland', 'Lower Lawrenceville', 'Bluff', 'Greenfield', 'Polish Hill', 'Central Oakland', 'Bloomfield', 'Hazelwood', 'South Oakland', 'Upper Hill', 'Shadyside', 'West Oakland', 'Squirrel Hill South', 'Terrace Village']
```

### Issues
---
If you run into any issues feel free to reach out to the UTAs or professors! We hope this helps.