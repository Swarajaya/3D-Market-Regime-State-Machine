3D Market Regime State Machine
What is this project about?

This project analyzes and visualizes stock market regimes (Bull, Bear, Sideways) using historical SPY data. It uses feature engineering, PCA for dimensionality reduction, and KMeans clustering to detect market states. The result is an animated 3D plot showing how market regimes evolve over time, with impressive visuals and clear regime transitions.

How to Fork

Click the "Fork" button at the top right of the GitHub repository page.

Clone your forked repository:

git clone https://github.com/Swarajaya/3D-Market-Regime-State-Machine.git


Navigate to the project directory and follow the setup instructions below.

Workflow

1. Download Data
Fetches SPY historical prices using yfinance.

2. Feature Engineering
Computes:

Rolling returns

Volatility

Momentum

Moving averages

3. Dimensionality Reduction
Uses PCA to project features into 3D space.

4. Clustering
Applies KMeans to detect market regimes.

5. Visualization
Animated 3D scatter plot with:

Colored regime points

Smooth rotation

Glowing effect

Regime transitions

Dark theme

Legend

Real-time timestamp

PCA & Clustering Explained

PCA (Principal Component Analysis)
Reduces the feature space to 3D while capturing the maximum variance in the data.

KMeans Clustering
Groups data into 3 clusters, labeled as:

Bull

Bear

Sideways

Labels are assigned based on mean returns of each cluster.

Project Structure
main.py               # Entry point  
regime_model.py       # Data processing, feature engineering, PCA, clustering  
visualization.py      # 3D animated visualization  
requirements.txt      # Dependencies  
README.md             # Project documentation  

Run the Project
1. Install Dependencies
pip install -r requirements.txt

2. Run
python main.py