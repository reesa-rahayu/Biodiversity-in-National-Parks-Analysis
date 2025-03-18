# National Parks Biodiversity Analysis

## Introduction

This project analyzes biodiversity fictional data from the National Parks Service provided by Codeacademy.com  to understand species distribution and conservation status across different national park locations. The goal is to explore patterns and answer questions related to species prevalence, conservation status, and observation counts.

**Key Questions Addressed:**

* What is the distribution of conservation status for species?
* Are certain types of species more likely to be endangered?
* Are there significant differences between species, their conservation status, and observation counts across parks?
* Which animal is most prevalent, and what is its distribution among parks?
* Which park has the highest total number of observations across all species?

**Data Sources:**

* `species_info.csv`: Contains information about species, including their category and conservation status.
* `observations.csv`: Contains observation data, including species observations in different national parks.

**Note:** The data is inspired by real data but is primarily fictional, provided by Codecademy.

## Setup and Dependencies

The project uses the following Python libraries:

* `pandas`: For data manipulation and analysis.
* `matplotlib`: For basic data visualization.
* `seaborn`: For enhanced data visualization.
* `scipy.stats`: For statistical analysis (chi-squared test).
* `re`: for regular expression operations.
* `itertools`: for efficient iteration.

## Data Exploration and Cleaning

* Loaded the `species_info.csv` and `observations.csv` datasets.
* Explored the data to understand the number of unique species, categories, and parks.
* Cleaned the `species` dataset by filling missing `conservation_status` values with "No Intervention."

## Data Analysis

### Distribution of Conservation Status

* Analyzed the distribution of conservation status across different species categories.
* Visualized the distribution using a stacked bar plot.
* Found that the majority of the species do not have conservation status.

### Endangered Species Analysis

* Identified endangered species and their distribution across categories.
* Visualized the distribution of endangered species using a bar plot.
* Calculated the percentage of protected species within each category.
* Used chi-squared test to determine if there is a statistical significance between the category of animal and the protection status.
* Found that mammals are most likely to be endangered.

### Species Prevalence and Distribution

* Extracted common names for each species category.
* Identified the most common species within each category (e.g., "Bat" for mammals, "Warbler" for birds).
* Analyzed the distribution of observations for the most common species across different parks.
* Visualized the distribution using bar plots.
* Found that Yellowstone national park has the highest number of species observations.

### Park Observation Analysis

* Analyzed the number of observation for uncommon species such as bear, and deer.
* Found that Yellowstone national park has the highest number of species observations.

## Key Findings

* Mammals have the highest proportion of endangered species.
* Yellowstone National Park has the highest total number of species observations.
* There is a statistically significant correlation between the animal category and the protection status for most of the animal categories.
* The most common animals are, Bat, Warbler, Snake, Salamander, Shiner, Sedge, and Moss for Mammal, Bird, Reptile, Amphibian, Fish, Vascular Plant, and Nonvascular Plant respectively.

## Conclusion

This analysis provides insights into the biodiversity of national parks, highlighting the distribution of conservation status, the prevalence of certain species, and observation patterns across parks. Further analysis could explore temporal trends in observations and the impact of environmental factors on species distribution.
