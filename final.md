# 1.Introduction  
**Oracle Arena** is the home stadium of NBA team Golden State Warriors.  
In the NBA home stadium and its surrounding stadium, usually sell the home team jersey and other peripheral products.  
For **different types** of surrounding sports venues, **different sales strategies** should be prepared.  
Need to **classify** the surrounding sports venues

---
# 2.Data

Data from **foursquare**.  
30 playgrounds near to Oracle Arena have been found  

---
# 3.Methodology

**K-means clustering algorithm** first randomly selects K objects as the initial clustering center.  
Then the distance between each object and each seed cluster center is calculated, and each object is assigned to the nearest cluster center.  
Cluster centers and objects assigned to them represent a cluster.   
Once all the objects are allocated, the cluster center of each cluster is recalculated according to the existing objects in the cluster.  
This process will be repeated until a termination condition is met.  
The termination condition may be that no (or minimum number) objects are reassigned to different clusters, no (or minimum number) cluster centers change again, and the sum of squares of errors is local minimum.

---
# 4.Result

Thirty stadiums are grouped into three categories  
![result](https://github.com/zhaoyuanfang/IBMDataScientist/result.jpg)  

---
# 5.Discussion
The result of the stadium classification seems to be based on the distance from the home court to Oracle Stadium. This result is based on the results of the current data set. If other factors, such as peripheral facilities, are taken into account, there may be other different results.  

---
# 6.Conclusion
The distance between the stadium and the main stadium is the main factor of classification, and the sales strategy of Jersey should be different for different stadiums.