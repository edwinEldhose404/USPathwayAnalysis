## 📁 Available Datasets -- Hosted on AWS

1. 🚀 CampaignPerformance.csv
2. 🎯 LeadsGenerated.csv
3. 📞 PhoneMetricsWithLeaveId.csv
4. 📱 PhoneMetricsWithoutLeaveId.csv
5. 💰 TokensPaidWithLeadID.csv
6. 💸 TokensPaidWithoutLeadID.csv
7. 👨‍💼 CandidateApplicationTrackerWithLeadIDs.csv
8. 👩‍💼 CandidateApplicationTrackerWithoutLeadIDs.csv

## 🛠 How to Use

To access these datasets, use the following Python function:

```python
# !pip install boto3
import pandas as pd
import boto3

def read_s3_dataset(file_name):
    s3_url = f"http://futurense-us-pathway-cleaned-datasets.s3-website-us-east-1.amazonaws.com/{file_name}"
    df = pd.read_csv(s3_url)
    
    return df

# Example usage:
data = read_s3_dataset("CampaignPerformance.csv")
```

## 📚 Dependencies

Make sure you have the following libraries installed:

```
boto3 (for extended AWS functionality)
```