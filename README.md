# Visualizing-Data-with-QuickSight-on-aws
<img width="705" alt="Architect-" src="https://github.com/user-attachments/assets/5866ca31-9401-465a-bd3e-7e72f788b072">
This project demonstrates the process of visualizing Netflix's data trends using **Amazon S3** and **Amazon QuickSight**. It provides insights into Netflix's titles through various graphical visualizations.

---

## Features
- Data storage and retrieval using **Amazon S3**.
- Visualization of datasets using **Amazon QuickSight**.
- Interactive visualizations like pie charts, bar graphs, and more.

---

## Getting Started

### Prerequisites
1. An **AWS account** with permissions for Amazon S3 and QuickSight.
2. A text editor (e.g., **VS Code**) to edit JSON files.

### Services Used
- **Amazon S3**: For storing datasets.
- **Amazon QuickSight**: For creating and exploring data visualizations.

---

## Steps to Implement

### Step 1: Download the Dataset
1. Download the necessary files:
   - [Netflix Dataset (CSV)](https://storage.googleapis.com/nextwork_course_resources/courses/aws/AWS%20Project%20People%20projects/Project:%20Visualise%20Data%20using%20Amazon%20QuickSight/netflix_titles.csv)
   - [Manifest File (JSON)](https://storage.googleapis.com/nextwork_course_resources/courses/aws/AWS%20Project%20People%20projects/Project:%20Visualise%20Data%20using%20Amazon%20QuickSight/manifest.json)

---

### Step 2: Upload the Dataset to Amazon S3
1. Create a new **S3 bucket**, e.g., `netflixx-pro`, in your preferred AWS region.
2. Upload the `netflix_titles.csv` and `manifest.json` files to this bucket.
3. Edit the `manifest.json` file:
   - Replace the URL placeholder with the **S3 URI** of the uploaded CSV dataset. For example:
     ```json
     "URIs": [
         "s3://netflixx-pro/netflix_titles.csv"
     ]
     ```
   - Save and re-upload the updated `manifest.json` file to S3.

---

### Step 3: Set Up Amazon QuickSight
1. Sign up for an **Amazon QuickSight** account.
2. Ensure your **S3 bucket** and QuickSight instance are in the same AWS region.
3. While signing up, uncheck the **Paginated Report** upgrade to avoid additional charges.

---

### Step 4: Connect S3 Bucket to Amazon QuickSight
1. In QuickSight, navigate to **Datasets** and select **New Dataset**.
2. Choose **S3** as the data source.
3. Enter a name (e.g., `Netflix Data`) and paste the S3 URI of the `manifest.json` file.
4. Complete the connection setup.

---

### Step 5: Visualize the Data
1. Use QuickSight’s interface to create visualizations:
   - Drag dataset fields into graphs.
   - Experiment with different chart types (e.g., pie charts, bar graphs, etc.).
2. Analyze insights such as:
   - Number of movies/TV shows by year.
   - Popular genres like "Thrillers" and "Action & Adventure."

---

## Project Files

| File Name           | Description                                              |
|---------------------|----------------------------------------------------------|
| `netflix_titles.csv` | Contains Netflix titles dataset in CSV format.          |
| `manifest.json`      | JSON file linking the S3 dataset with Amazon QuickSight.|

---

## Visual Examples
### Example Insights
- Movies and TV shows distributed by release year.
- Popular genres over time.
- Comparison of movies vs. TV shows.
[Sheet_1_2024-08-12T17_51_47.pdf](https://github.com/user-attachments/files/17804461/Sheet_1_2024-08-12T17_51_47.pdf)
<img width="1669" alt="Visualise Architect" src="https://github.com/user-attachments/assets/2e0a9748-cc1d-4c35-82a6-9314654536d5">




---

## Notes
- Ensure the dataset is up-to-date for accurate visualizations.
- Monitor your AWS services to avoid unexpected charges.

---

## References
- [Amazon S3 Documentation](https://docs.aws.amazon.com/s3/)
- [Amazon QuickSight Documentation](https://docs.aws.amazon.com/quicksight/)
- Dataset Source: [https://www.kaggle.com]
---


---
