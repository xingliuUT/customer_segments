# Machine Learning Engineer Nanodegree
## Project: Creating Customer Segments

### Code

The code is in the `customer_segments.ipynb` notebook file. Visualization code is in `visuals.py` Python file. Data for this project is contained in the `customers.csv` dataset file.

### Run

```bash
jupyter notebook customer_segments.ipynb
```

## Data

The customer segments data is included as a selection of 440 data points collected on data found from clients of a wholesale distributor in Lisbon, Portugal. More information can be found on the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Wholesale+customers).

Note (m.u.) is shorthand for *monetary units*.

**Features**
1) `Fresh`: annual spending (m.u.) on fresh products (Continuous); 
2) `Milk`: annual spending (m.u.) on milk products (Continuous); 
3) `Grocery`: annual spending (m.u.) on grocery products (Continuous); 
4) `Frozen`: annual spending (m.u.) on frozen products (Continuous);
5) `Detergents_Paper`: annual spending (m.u.) on detergents and paper products (Continuous);
6) `Delicatessen`: annual spending (m.u.) on and delicatessen products (Continuous); 
7) `Channel`: {Hotel/Restaurant/Cafe - 1, Retail - 2} (Nominal)
8) `Region`: {Lisbon - 1, Oporto - 2, or Other - 3} (Nominal) 

## Conclusion

Apply PCA to find 2 principle components to fit model, which explained about 74% of the variance of features. K-Means Clustering method with 2 clusters is used and achieves the silhouette score of 0.4263. 

These analysis confirms with the `Channel` feature that was excluded from the data in the beginning. The customers has two segments: Hotel/Restaurant/Cafe and Retail. 

One way to make use of the customer segments information, A/B test on delivery schedule is briefly discussed.
