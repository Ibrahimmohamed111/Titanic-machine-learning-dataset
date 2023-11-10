Prepare the data
Download the data. The image mentions that the data is available in a CSV file. We can use the following code to download the data:
import requests

# Download the data from the CSV file link
url = "https://example.com/titanic_data.csv"
response = requests.get(url)

# Save the data to a local file
with open("titanic_data.csv", "wb") as f:
    f.write(response.content)
