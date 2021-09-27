---
title: Query sample data 
description: >
  Explore InfluxDB Cloud with our sample data buckets. 
menu:
  influxdb_cloud:
    name: Query with sample data
    parent: Execute queries
weight: 10
---

Use **InfluxDB Cloud** sample datasets to quickly access data that lets you explore and familiarize yourself with InfluxDB Cloud without requiring you to have or write your own data.

- [Add a sample data](#add-a-sample-data)
- [Explore sample data](#explore-sample-data)
- [View demo sample dashboards](#view-demo-data-dashboards)

{{% note %}}
#### Network bandwidth

Each execution of `sample.data()` downloads the specified dataset from **Amazon S3**.
If using [InfluxDB Cloud](/influxdb/cloud/) or a hosted InfluxDB OSS instance,
you may see additional network bandwidth costs when using this function.
Approximate sample dataset sizes are listed for each [sample dataset](/influxdb/cloud/reference/sample-data/#sample-datasets) and in the output of [`sample.list()`](/influxdb/v2.0/reference/flux/stdlib/influxdb-sample/list/). To 
{{% /note %}}

## Add sample data

1. Choose from the following sample datasets:
   - **Air sensor sample data**: Explore, visualize, and monitor humidity, temperature, and carbon monoxide levels in the air.
   - **Bird migration sample data**: Explore, visualize, and monitor the latitude and longitude of bird migration patterns. 
   - **NOAA NDBC sample data**: Explore, visualize, and monitor NDBC's observations from their buoys. This data observes air temperature, wind speed, and more from specific locations. 
   - **NOAA water sample data**: Explore, visualize, and monitor temperature, water level, pH, and quality from specific locations. 
   - **USGS Earthquake data**: Explore, visualize, and monitor earthquake monitoring data. This data includes alerts, cdi, quarry blast, magnitide, and more.  
2. Do one of the following to download sample data: 
   - [Install community templates](#add-sample-data-with-community-templates) 
   - [Download using the InfluxDB UI](#add-sample-data-with-influxdata-ui)
   - [Create a template](#add-sample-data-with-templates)

### Add sample data with community templates

1. Go to the [GitHub community templates sample data](https://github.com/influxdata/community-templates/tree/master/sample-data) page. 
2. Follow the instructions listed under **Quick Install**.

### Download using the InfluxDB UI

1. Go to **Explore > Script Editor**.
2. Put your sample data query from the 

## Sample data sets

Choose from the following sample datasets:

- **Air sensor sample data**
  - Explore, visualize, and monitor humidity, temperature, and carbon monoxide levels in the air.
- **Bird migration sample data**
  - Explore, visualize, and monitor the latitude and longitude of bird migration patterns.
- **NOAA NDBC data**
  - Explore, visualize, and monitor NDBC's observations from their buoys. This data observes air temperature, wind speed, and more from specific locations.
- **NOAA water sample data**
  - Explore, visualize, and monitor temperature, water level, pH, and quality from specific locations.
- **USGS Earthquake data**
  - Explore, visualize, and monitor earthquake monitoring data. This data includes alerts, cdi, quarry blast, magnitude, and more.

For more information, see our [sample data](/influxdb/cloud/reference/sample-data/).

## Explore sample data
Use the [Data Explorer](/influxdb/cloud/visualize-data/explore-metrics/)
to query and visualize data in sample data buckets.

In the navigation menu on the left, click **Explore (Data Explorer)**.

{{< nav-icon "explore" >}}

## Add sample data

1. In the navigation menu on the left, click **Data (Load Data)** > **Buckets**.

    {{< nav-icon "data" >}}

2. Click **{{< icon "plus" >}} Create bucket**, and then name your bucket. The bucket will appear in your list of buckets.
3. View the [sample datasets document](/influxdb/cloud/reference/sample-data/#sample-datasets) and choose a sample data to query.
4. Copy the `sample.data()` function listed underneath.
5. Click **Explore** on the left navigation of InfluxDB Cloud and click your bucket, and then click **Script Editor**.
6. Paste the `sample.data()` function.
7. Click **Submit** to run the query.

## Create sample data dashboards
After adding a sample data bucket, create a dashboard specific to the sample dataset:

1. Click **Boards (Dashboards)** in the navigation menu on the left.

    {{< nav-icon "dashboards" >}}

2. Click **Create Dashboard > New Dashboard**, and name the dashboard after your bucket. 
3. Click **Add Cell**, and select your sample data bucket.
4. Click **Script Editor**.
5. Copy and paste the `sample.data()` function into the script editor.
6. Click **Submit** to run the query.
6. Define the variables of your sample data.
