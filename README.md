# Autonomous RFID Robot

This project involves the development of an autonomous robot, having RFID capabilities for tracking assets. The two major aspects of this project includes both signal processing and fabrication. The signal processing was handled with `Python`, where the robot was equipped with an RFID reader, receiving backscatter signals from different tags in the environment. These signals were then processed using two main localization algorithms, being received signal strength indicator (RSSI) and phase. The robot's job is then to traverse the environment and sample all RFID tags, which will use the localization algorithms to calculate where each are located.

To handle the processing of high-density RFID tags in an arbitrary environment, APIs were developed using `FastAPI` with `Elasticsearch` to provide real-time updates. `Elasticsearch` is the database of choice in this case due to its ability to handle large data aggregations with full-text search, beneficial with querying a large number of assets.

Below is a high-level block diagram that shows how the main components were organized:

![diagram](./diagram.png)

**NOTE**: Unfortunately, the code for this project is proprietary and cannot be shared publically. If you want to learn more about this project, feel free to reach out to me.