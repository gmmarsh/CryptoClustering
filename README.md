# Crypto Clustering

This project aims to develop an unsupervised machine learning model for clustering crypto currencies. The K-Means model was fit on a dataset of historical crypto currency market data.

## Table of Contents
- [Introduction](#introduction)
- [Data](#data)
- [Methodology](#methodology)
- [Results](#results)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction
Unsupervised machine learning clustering is important because hidden patterns can be discovered. This can lead to new insights and understanding of the crypto currency data. Clustering can be used to detect outliers or anomalies as well. Clustering can be used to simplify a large dataset making the data easier to analyze and visualize.

## Data
The dataset used for this project consists of historical crypto currency market data, including features such as coin id, price changes as a percentage for 24 hours, 7 days, 14 days, 30 days, 60 days, 200 days and 1 year. The dataset was preprocessed and was fit to the SKLearn K-Means model.

## Methodology
After preparing the original dataset using SKLearn's Standard Scaler, the optimal value for "k" was found using the "elbow curve" inertia methology. The optimal value for "k" was determined to be four. The K-Means model was fit to the scaled data and scatter plot was used to depict the clustered coin ids.

Principal component analysis was used to reduce the number of input features in the dataset to three input features allowing for easier visualization and reducing the noise in the dataset by discarding components that capture less variance. A k value using the "elbow curve" inertia methodology was used again and the optimal value for "k" was determined to be four again.

Finally, the K-means cluster visualizations for the original data set and the principal component analysis were compared. 

## Results

After visually analyzing the cluster analysis results, the PCA clustering algorithm produces more distinct clusters. The Calinski-Harabasz Index is higher for the PCA data algorithm further reinforcing the conclusion of the visual analysis.

## Usage
To use this project, follow these steps:
1. Clone the repository: `git clone https://github.com/gmmarsh/credit_risk_classification.git`
2. Install the required dependencies: `pip install -r requirements.txt`
3. Run the main script: `Crypto_Clustering.ipynb`

## Contributing
Contributions to this project are welcome. If you find any issues or have suggestions for improvement, please open an issue or submit a pull request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.