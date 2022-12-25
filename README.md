# Commodity_deep_stacked_LSTM
To predict London Metal Exchange(LME) Aluminium price (in MT/Tonne) using a deep stacked LSTM. 
The London Metal Exchange (LME) is a futures and forwards exchange with the world's largest market in standarised forward contracts, futures contracts and options on base metals. The exchange also offers contracts on ferrous metals and precious metals. 
The Features used here for building the model are:
1. LME Aluminium
2. LME stock (in LME approved warehouses)
3. LME Copper
4. LME Zinc
5. Coal prices
The data has been collected from the following links:
LME Aluminium and LME Stock- https://www.westmetall.com/en/markdaten.php?action=table&field=LME_Al_cash
LME Copper - https://www.westmetall.com/en/markdaten.php?action=table&field=LME_Cu_cash
LME Zinc - https://www.westmetall.com/en/markdaten.php?action=table&field=LME_Zn_cash
Coal - https://in.investing.com/equities/coal-india-historical-data
To predict the LME Aluminium (commodity price), other commodity prices have been used. Also, since Aluminium is an energy intensive material, coal proces are also taken into consideration.
The data is pre-processed, removing missing values, scaling the input
To build the model, datastructure is created with 60 timesteps to predict the LME Aluminium price on the required day
