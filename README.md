# NBA Shot Logs Analysis
This project analyzes NBA shot logs data to gain insights into player performance, team statistics, and shooting patterns. It leverages PySpark, machine learning techniques, and MapReduce algorithms to explore correlations, predict field goal outcomes, identify outliers, and determine team MVPs.

## Dataset

The dataset used in this project can be found on [Kaggle](https://www.kaggle.com/datasets/dansbecker/nba-shot-logs). It provides comprehensive information about NBA shots, including shot distance, shot clock time, dribbles, defender distance, and shot result.

## Project Steps

1. **Data Preprocessing**: Clean the dataset by handling missing values, replacing negative values, and converting the GAME_CLOCK format into seconds.

2. **Data Correlation Visualization**: Explore correlations between features and the FGM (Field Goal Made) column to identify factors influencing shot success.

3. **Outlier Analysis**: Visualize outliers in the dataset and make informed decisions on their treatment based on their significance for analysis.

4. **Partition Clustering**: Apply partition clustering on selected features, such as SHOT_CLOCK, DRIBBLES, SHOT_DIST, CLOSE_DEF_DIST, TOUCH_TIME, and SHOT_RESULT, with 5 clusters.

5. **Partition Clustering Visualization**: Visualize the results of partition clustering to understand the grouping of data points.

6. **Classification Models**: Employ four classifiers—Random Forest, GBT (Gradient Boosting), Linear Regressor, and Logistic Regressor—to predict the FGM column using features such as SHOT_DIST, TOUCH_TIME, CLOSE_DEF_DIST, and SHOT_CLOCK.

7. **MapReduce Functions**: Implement three MapReduce functions:
   - Winning Teams Shooting Percentage: Calculate the shooting percentage for winning teams in each GameID.
   - Player's Average Shooting Distance: Calculate the average shooting distance for each player in each game to analyze shooting preferences.
   - Most Valuable Players (MVP) in Each Team: Identify the MVP player in each team based on successful dribbles and shots made.

8. **Big Data Market Analysis**: Utilize the Chi-square test for association rule analysis to identify features that are dependent on each other, such as 'SHOT_RESULT', 'PERIOD', 'DRIBBLES', 'CLOSE_DEF_DIST', and 'SHOT_DIST'.

## Installation

To run the project, it is recommended to use Python 3.9 and JDK 17. For installation instructions for PySpark and Hadoop on Windows, refer to this [YouTube tutorial](https://www.youtube.com/watch?v=OmcSTQVkrvo&t=689s&ab_channel=AmpCode).

## Usage

1. Clone the repository:
   ```shell
   git clone https://github.com/YousefGaafer/NBA-Shot-Logs-Analysis.git
   ```

2. Install the required dependencies:
   ```shell
   pip install -r requirements.txt
   ```

3. Run the Jupyter Notebook or Python scripts to execute the different steps of the project.

## Contributing

Contributions are welcome! Please feel free to open an issue or submit a pull request.

## Authors

- Author 1: [Yousef Gaafer](https://github.com/YousefGaafer)
- Author 2: [Mohamed Wael](https://github.com/MohamedWZS)
- Author 3: [Ziad Mansour](https://github.com/ZiadMansourM)

## Acknowledgments

We would like to acknowledge the [NBA](https://www.nba.com/) for providing the shot logs dataset of 2015 season.

## References

- [Kaggle: NBA Shot Logs Dataset](https://www.kaggle.com/datasets/dansbecker/nba-shot-logs)
- [PySpark Documentation](https://spark.apache.org/docs/latest/api/python/)
- [YouTube Tutorial: PySpark and Hadoop Installation on Windows](https://www.youtube.com/watch?v=OmcSTQVkrvo&t=689s&ab_channel=AmpCode)
