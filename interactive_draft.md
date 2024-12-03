# Global Migration Flows

Magdalena Barrps

## What is your current goal? Has it changed since the proposal?

My goal is to create an interactive visualization that raises awareness about global migration patterns. The project combines a quiz, an icon-based visualization, and a world map with migration filters to provide an engaging and educational experience. The focus remains on improving user interaction and understanding the migration data in a meaningful way.

## Are there data challenges you are facing? Are you currently depending on mock data?

Yes, I am currently relying on mock data to prototype the visualizations and interactions.

Also there are several data challenges I am facing:

1. **Filters for "From" and "To"**: Implementing these filters in a way that dynamically hides or displays points based on user selection has been challenging. The goal is to ensure that the map updates seamlessly, showing only the relevant data based on the selected countries.

2. **Multi-Country Selection**: Allowing users to select more than one country for "From" and "To".

3. **Simulating Point Movement Across Countries**: Applying the animation of points moving between multiple countries simultaneously is a technical challenge.

4. **Incorporating Multiple Years**: Adding a timeline or year filter to show migration patterns over different years requires designing a structure that handles time-series data effectively while keeping the map responsive and user-friendly.

## Walk us through an interaction, either in words or you can record a quick 2-3 minute video.

The interaction begins with a quiz about migration facts, engaging users with questions that encourage reflection on global migration trends. After completing the quiz, the user scrolls down to see an icon-based visualization. This section uses person-shaped icons to represent population data. Over time, specific icons are highlighted to reflect the percentage of migrants, dynamically changing as the user selects different years.

Finally, a world map visualization appears. The map allows users to filter migration data using "From" and "To" dropdowns. Users can select one or more countries to view the migration flows, with points dynamically animating to represent migration movement between the selected countries over time.

## Include a _numbered_ list of questions for us to respond to.

1. How can I better implement the "From" and "To" filters to dynamically hide points and allow multi-country selection?
2. What would be the best approach to simulate point movement between multiple countries in a visually coherent way?
3. Are there any suggestions for structuring or visualizing time-series data for the migration map effectively?
4. Does the combination of quiz, icon visualization, and map provide a cohesive user experience? If not, how can it be improved?



# References

1. https://observablehq.com/@neocartocnrs/dot-density-map-from-countries
2. https://observablehq.com/@floledermann/dot-density-maps-with-d3
3. https://github.com/d3/d3-geo-projection/blob/main/README.md
4. https://observablehq.com/@d3/walmarts-growth
5. https://d3js.org/d3-polygon
6. https://worldmigrationreport.iom.int/wmr-2022-interactive/
7. https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/random



