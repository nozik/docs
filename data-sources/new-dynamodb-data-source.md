# New DynamoDB Data Source

DynamoDB is an Amazon Web Services \(AWS\) database system that can be integrated easily with build.security as a data source for implementing your authorization policies. Based on the policies defined in build.security and the information provided by the data source, the PDP can determine the authorization decision.

**To create a DynamoDB data source in the control plane:**

1. Click the **NEW DATA SOURCE** button on the data source screen. The New Data Source panel will open on the right.
2. In the **Name** field, enter the name of the new data source.
3. In the **Description** field, enter a description \(optional\).
4. In the **Type** area, select **DynamoDB**.
5. In the **AWS Region** field, you can either select a region or leave the default value of "Auto discovery," allowing build.security to automatically determine the relevant region.
6. In the **Access Key Environment Variable** field, enter the environmental variable that will hold the access key for the DynamoDB data source, or leave it blank for auto-discovery.
7. In the **Secret Access Key Environment Variable** field, enter the environment variable that iwll hold the secret access key, or leave it blank for auto-discovery. After creating the Dynamo data source, you will need to declare this variable to [deploy the PDP](https://docs.build.security/docs/deploying-a-pdp).
8. In the **Consistent Read** field, choose whether to enable consistent read. When enabled, the DynamoDB will return a response with the most up-to-date data. The default value is disabled. To read more about this DynamoDB feature, see [AWS documentation on Read Consistency](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/HowItWorks.ReadConsistency.html).
9. In the **Cache TTL** field, enter the amount of time the cache memory of queries retrieved from the databases to the PDP will be cached and available for the PDP. Acceptable values \(in seconds\) is 0-600.
10. Click **SAVE** to create the new data source.

The new DynamoDB data source will now appear in the list of existing data sources on the data source screen.

![New DynamoDB data source](https://files.readme.io/14c236a-newdynamodb.PNG)



