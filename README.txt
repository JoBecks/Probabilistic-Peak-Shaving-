Project Organization


├── README.md          			<- README for organization overview.
├── code
│   ├── FCR_market_code.ipynb       	<- Script for modeling the FCR market price
│   ├── Q-LSTM_code.ipynb        	<- Tuning, training and testing the Q-LSTM. Also transforms output into forecast
│   ├── Regulation_signal_code.ipynb	<- Script for modeling the regulation signal      
│   └── Simulation_code.ipynb    	<- Script for simulation of one year        
│
├── data                
│   ├── consumption_data         	<- Net consumption load data of the companies
│   │   │      
│   │   ├── interim           		<- Intermediate data that has been transformed
│   │   ├── processed			<- Final dataset with all information needed for probabilistic forecasting
│   │   └── raw				<- Original dataset 
│   │
│   ├── FCR_market_data  		<- FCR market data from 2019 - 2021 
│   ├── forecast_data			<- Final output of the Q-LSTM: Probablistic forecasts
│   ├── hyperparameter_and_loss_data    <- Raw output of the Q-LSTM: Chosen hyperparameters, test loss and normalized forecast data
│   └── regulation_signal_data		<- Regulation signal data in 1s resolution from 2019 - 2021
│
└── requirements.txt			<- requirements for the venv for running the scripts
