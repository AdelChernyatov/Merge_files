# Merge_files
Processing and merging two files from sensor and mobile(for large amount of data)

## Getting Started
Run the kernel in file_process.ipynb

  ### Prerequisites
  Python(3.11.4 or higher)
  
  Numpy(1.25.2 or higher)
  
  Pandas(2.0.3 or higher)

  ### Installation
  Clone the repository: https://github.com/AdelChernyatov/Merge_files.git
  
  Navigate to the project directory: cd Merge_files
  
  Install dependencies: pip install -r requirements.txt

## Usage
storage_data is a directory, where you need move your sensor and mobile data files
1) in a row write_csv(log_filename = storage_data/your_sensor_name.log, csv_filename = storage_data/sensor.csv) -
2) mobile_df = pd.read_csv('sensor_output/Raw Data.csv') - magnetic field mobile values without date
3)  mobile_time_df = pd.read_csv('storage_data/time.csv') - date of measurements
4)  extract_df = pd.read_csv('storage_data/sensors.csv') - magnetic field sensor values with date

mobile_sensor_output - final merged dataframe with both values
