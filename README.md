# Airbnb Listing Quality Analysis

## Project Overview
This project analyzes Airbnb listings data to create a scoring system for determining the quality of listings from a host's perspective. The goal is to understand what qualifies as a good listing and to predict whether a listing is bad, average, or good.

## Dataset
The analysis uses the Airbnb listings dataset for London, which includes information about properties, hosts, pricing, and reviews.

## Methodology

### Data Preprocessing
- Converted relevant columns to appropriate data types
- Filtered and cleaned the dataset
- Removed outliers in pricing

### Feature Engineering
1. **Host Attributes**:
   - Superhost status
   - Host ratings
2. **Property Attributes**:
   - Amenities
   - Accommodates
   - Property ratings
3. **Pricing**:
   - Competitive pricing analysis

### Scoring System
A composite score was created based on:
- Superhost score
- Host review score
- Listing review score
- Competitive pricing score
- Amenities score

### Model Development
- Used multinomial logistic regression to predict listing quality
- Split data into training (75%) and testing (25%) sets

## Key Findings
- The final score ranges from 5.5 to 65, with a maximum achievable score of 73
- Listings are categorized into three tiers: bad, average, and good
- The model achieved an accuracy of 80%, with better performance in predicting the highest and lowest quality listings

## Challenges and Future Improvements
- Improve prediction accuracy for average quality listings
- Incorporate additional external data sources
- Explore alternative modeling techniques (e.g., decision trees, random forests)

## Libraries Used
- dplyr
- tidyr
- ggplot2
- zoo
- rpart
- readr
- nnet
- caret
- coefplot
- pROC

## How to Run
1. Ensure all required libraries are installed
2. Set working directory to the project folder
3. Run the R Markdown file

## Contributors
[Your Name]

## License
[Specify your license here]
