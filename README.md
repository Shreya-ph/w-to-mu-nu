# w-to-mu-nu

Overview:
The analysis is based on the cms data from CERN opendata. The data contains 100k events where one muon candidate was observed and missing energy implies to the presence of a neutrino. The data is a subset of the total event information from the primary dataset SingleMu 2011. They are not suitable for a full physics analysis. This project is strictly exploratory and lacks any significant implications due to the nature of the data. 
The muon momentum, Missing momentum and phiMET, transverse mass are plotted as histograms. The transverse mass observable has been reconstructed from event-level data and train an XGBoost regressor to predict it from kinematic features. XGBoost successfully learns the analytic mapping from event-level features to transverse mass.

Methods and tools:
1.	Numpy
2.	Matplotlib
3.	Sklearn
4.	Mpl_toolkits
5.	Xgboost

Limitations:
1.	Only transverse observables are used, full invariant mass reconstruction not possible.
2.	The data is a subset of the total event information from the primary dataset SingleMu 2011. They are not suitable for a full physics analysis

References:
1.	https://opendata.cern.ch/record/5205
