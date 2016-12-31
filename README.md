# tomcat8-rediscluster-session-manager

Currently the "tomcat-redis-session-manager" from "jcoleman" is not supported for Tomcat 8 and redis cluster 3.x.
So gathered both two feature and integrated into one.

Please pay attention. <br>

When do configuration for redis non-cluster session manager. please use below pair.<br>
&#x3C;Valve className="com.orangefunction.tomcat.redissessions.RedisSessionHandlerValve" /&#x3E;<br>
&#x3C;Manager className="com.orangefunction.tomcat.redissessions.RedisSessionManager" "..."/&#x3E;
<br>
<br>
when do configuration for redis cluster session manager, please use below pair.<br>
&#x3C;Valve className="com.orangefunction.tomcat.redissessions.RedisClusterSessionHandlerValve" /&#x3E;<br>
&#x3C;Manager className="com.orangefunction.tomcat.redissessions.RedisClusterSessionManager" "..."/&#x3E;<br>
<br>
for more configuraion details, please refer below.
<br>
<br>
Reference for redis cluster approache<br>
[https://github.com/zhmz1326/tomcat-redis-session-manager.git]<br>
<br><br>
Reference of original approach<br>
[https://github.com/jcoleman/tomcat-redis-session-manager.git]<br>
<br>
<br>
<br>

Please note - This version is only tested in some limited area. So please take into consideration before introduce it into PRODUCTION environment. <br> 
<br>
And also, I'm very happy to know if you find any issue during your testing.
<br>
<br>
Br, <br>
(Bob) XuYong Hou
