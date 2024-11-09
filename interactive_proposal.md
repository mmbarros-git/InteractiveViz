# Proposal for Interactive Visualization on Global Migration Flows

Magdalena Barros

## Description of the Topic and Data

I am planning to explore the topic of global migration flows, focusing on the 
movement of people between countries over time. The data I will use is from 
the **United Nations Department of Economic and Social Affairs (UNDESA)**, which 
provides estimates of international migration flows by country. This dataset includes 
migration data disaggregated by age, sex, and country or area of origin. 
It also presents annual migration flows, including both immigration and emigration, 
for various countries.

### Data Sources:
1. **International Migration Flows** - [UN DESA Migration Data](https://www.un.org/development/desa/pd/data/international-migration-flows)
   - This dataset contains migration flow data from 1990 to 2020, including data on emigration, immigration, asylum seekers, and stocks of foreign populations, providing insights into global migration trends.

2. **File: undesa_pd_2015_migration_flow_totals** (Uploaded)
   - This file provides migration flow totals for different countries over several years, 
   giving valuable data on international movement for countries across the globe. 
   Data from 1980 to 2013, 45 unique countries inmigration and migration. 

3. **File: undesa_pd_2020_ims_stock_by_sex_destination_and_origin** (Uploaded)
   - This dataset provides stock data for international migrants by sex, destination, and origin, covering data on the number of international migrants for various countries and regions.
   It also includes estimates for international migrant stocks segmented by sex and origin, offering a detailed view of migration patterns. This data is essential for understanding the composition and flow of international migration and can be used to analyze changes in migration dynamics from 1990 to 2020.

---

## Examples of Interactive Visualizations

I have reviewed several interactive visualizations that could guide the design of the project:

1. **Make Your Own Mobility Animation** – [New York Times](https://www.nytimes.com/interactive/2018/03/27/upshot/make-your-own-mobility-animation.html)
   - **Description**: This interactive visualization allows users to explore social mobility by simulating the movement of people from one income level to another, based on their socio-economic background and race. It shows how individuals born into various economic conditions (e.g., poor, rich, or middle-class) move through different income brackets over time, providing insights into the impact of race and starting conditions on economic outcomes.
   - **Application to My Data**: I envision using this concept for showing migration flows between countries. The countries would be represented on the map, and the points representing the migration flow would move dynamically as the years pass.

2. **A Day in the Life of Americans** – [Flowing Data](https://flowingdata.com/2015/12/15/a-day-in-the-life-of-americans/)
   - **Description**: This interactive shows movement patterns by using animated points. Each point represents an individual, and the animation illustrates their movements over time.
   - **Application to My Data**: I plan to use this idea for depicting migration data, where each point represents a migrant's movement from one country to another. The animation will show how migration trends evolve year by year.

3. **Interactive Migration Data Visualization** – [International Organization for Migration (IOM)](https://worldmigrationreport.iom.int/wmr-2022-interactive/)
   - **Description**: This tool allows users to explore various migration data points across multiple regions, presenting data in an interactive way with multiple layers of information.
   - **Application to My Data**: This approach will help enhance the analysis by enabling users to explore migration flows, compare immigration vs. emigration patterns, and explore migration across different years.

---

## How I Plan to Approach the Data

I plan to use **D3.js** to create an animated world map showing migration flows over time. Here’s how I envision the visualization:

- **Core Concept**: The map will display countries as nodes, with points representing the migration flows. As time progresses, these points will move between countries to show migration (both inflows and outflows). The data from the provided sources will be used to animate these movements, illustrating trends of immigration and emigration.
  
- **Interaction**: Users will be able to:
  1. Select a country to visualize the specific migration flows (inflow and outflow) for that country.
  2. Adjust the time frame to view migration patterns for specific years.
  3. Hover over countries or migration points to see the migration numbers for each flow (e.g., number of people migrating in or out).
  
- **Timeline**: As time passes, the migration points will move, allowing users to see how migration trends evolve year by year.

### Which Option Best Fits

This project fits best with **Option A**: **Core Interactive**. The focus will be on a single major visualization — the animated world map. The map will display countries as nodes, with points representing migration flows. Each point will correspond to a portion of the population, and as time progresses, these points will move between countries to show migration (both inflows and outflows). The number of points in each country will be proportional to its population, ensuring that larger countries have a higher density of points, which will visually represent the population concentration.

The migration flows will be animated over time, showing the dynamic movement of people between countries, indicating both immigration and emigration trends. The data from the provided sources will be used to animate these movements. Calculations will be made to ensure that the concentration of points in each country accurately reflects population size, and as migration occurs, the distribution of points will change, offering a visual representation of how migration patterns shift over time. This dynamic visualization will help users understand the scale and direction of migration flows globally.

---

## Questions for Feedback

1. How can I optimize the performance of the animation, especially if the dataset is large (e.g., many countries and years)?
2. Is it better to use **D3.js** for this project, or would a different library be more appropriate for handling large geographical datasets with animations?
3. Should I focus only on specific regions (e.g., Europe, North America), or is it better to include a global view and let users zoom into regions of interest?
4. Is the data presented in the Excel file adequate for creating the animation, or would it be better to include additional demographic details (e.g., age, gender)?

---

## Mock-up of Visualization

![Mock-up](/Users/magdalenabarros/InteractiveViz/mock_up/drawing.svg)

---

