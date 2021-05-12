## IoT Health Monitoring and Analytics
When the connected infrastructure is deployed at scale (100s of 1000s of devices), it is important to monitor the health of the end to end pipeline so that proactive actions can be taken to address any problems in the systems deployed in the field. This will include:

Collecting appropriate health parameters from each end node - Zenatix already collects such parameters from all its systems.
Separating out the health information (e.g. RSSI) from application information (e.g. temperature data) at the edge side - Currently all the health and application information is combined and sent to the same pipeline on the cloud.
Collecting additional health information from the edge gateway - Zenatix already collects multiple such parameters.
Creating a separate pipeline for health information which addresses typical requirements such as timeseries storage, log storage, developing meaningful dashboards on that data, purging rules to delete data after a certain time etc. - Zenatix currently has this mixed up with application pipeline in cloud and we would like to separate out the whole health monitoring and analytics.
Beyond monitoring the health information of the IoT hardware deployed in the field, it will be desirable to extend the same system for monitoring the software applications running both on the edge and the cloud.
Create suitable dashboards for the account management team at Zenatix which can help them to get a quick high level overview of performance of the systems deployed for a customer so as to have improved customer engagement - this will require developing systems in a way that custom queries and custom UI elements can be easily added in the future.
There are several open source tools available - such as ELK stack or TICK stack or Prometheus based logging. The project will involve understanding Zenatix stack, performing some PoCs with these open source monitoring and logging tools and then suitably modifying one such tool to address the requirements laid out for health monitoring and analytics at Zenatix.
