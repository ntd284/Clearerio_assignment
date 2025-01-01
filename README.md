
![db_diagram](images/db_diagram.png)

![flow](images/flow.png)

![dashboard](images/dashboard.png)


### 2. Challenges and Solutions in Multi-Region Data Migration to a Data Warehouse (DWH)

#### Timezone Differences Across Regions:
Problem: Timezone differences can cause inconsistencies in time-sensitive data, leading to errors in reporting, analytics, and scheduling jobs.
Solution: Carefully verify the timezone of data fetched from new regions. Convert all timestamps to UTC if not already standardized. After processing, create timezone-specific views for end-users based on the requirements of different applications.

**Data Format and Structural Differences:**
    **-Problem:** Variations in data formats and model structures across regions can lead to integration issues and potential data loss.
    **-Solution:** Verify and transform data to align with the DWH's existing format. Ensure robust data validation and transformation processes to avoid loss or corruption during migration.

**Latency and Data Synchronization:**
**Problem:** Migrating data across regions may introduce latency, impacting real-time reporting and synchronization between systems.

**Solution:** Position servers strategically based on customer locations. Utilize cloud providers' edge locations (small data centers distributed globally) to cache data and reduce latency for better real-time performance.

**Cost Management:**
**Problem:** Operating cross-region servers can incur high costs due to data transfer and resource usage.

**Solution:** Leverage cost-efficient regions for hosting services, as pricing varies between cloud regions. Evaluate and balance cost savings against latency to ensure an optimal solution.

**Compliance with Local Regulations:**
**Problem:** Some countries mandate that customer data from their region must be stored within their borders, necessitating compliance with local laws.

**Solution:** Host servers within the respective countries to meet regulatory requirements while maintaining secure and compliant data handling processes.