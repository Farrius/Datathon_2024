# Preprocessing

- Renombrament
- Remove attributes indicating the number of kitchens, bathrooms, and drawing rooms due to their ambiguity.
- Set the number of living rooms (bedrooms were mistranslated to living rooms) in a range from 1 to 4.
- Add attribute “distance” indicating the distance of the house from the center of Beijing.
- Replace attribute “constructionTime” with attribute “age” by deducting the year that the house was constructed from the current year (2019).
- Set minimum values for attributes “price” and “area”.
- Split the attribute “floor” into attributes “floorType” and “floorHeight”.
- Treat outliers.
- Irrelevant factors with minimal impact on rent were removed using an Excel spreadsheet.
- Add a new variable called ”total-ssvalue” to facilitate subsequent modeling (This variable represents the cumulative count of various soft furnishing facilities such as air conditioning, heating, and other amenities.).
- Variable square footage seems very important.
- Add categorical variables for the different types of buildings, such us we put 1 or 0 depending on the type. This works better for the RF.
- If entry does not have the price, remove it (since the entry will not be useful for the analysis).
- Impute missing variables
