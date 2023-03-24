# sidemen_analysis (Qazi Muneeb Shabir)

This code is a Python script that uses the Google YouTube Data API to retrieve statistics for a list of YouTube channels belonging to the Sidemen group, and then visualizes the data using the Seaborn library.

The script begins by importing the necessary libraries: googleapiclient.discovery, pandas, and seaborn. It then defines an API key and a list of channel IDs for the Sidemen group.

Next, a function get_channel_stat() is defined, which takes in the YouTube object and the list of channel IDs as inputs. The function uses the youtube.channels().list() method to request data for each channel in the list, and extracts the relevant information such as the channel name, subscriber count, view count, and total video count. The function then returns a Pandas DataFrame containing this information for all the channels.

The get_channel_stat() function is called with the YouTube object and the list of channel IDs as arguments to retrieve the channel statistics data.

The script then converts the 'Subscriber Count', 'Views', and 'Total Videos' columns in the DataFrame to numeric data types using the pd.to_numeric() method.

Finally, the Seaborn library is used to create a bar plot visualization of the subscriber counts for each channel in the DataFrame. The sns.set() method is used to set the size of the plot, and the sns.barplot() method is used to create the actual plot.
