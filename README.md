# tomcat8-rediscluster-session-manager

Currently the "tomcat-redis-session-manager" from "jcoleman" is not supported for Tomcat 8 and redis cluster 3.x.
So gathered both two feature and integrated into one.

Please pay attention.

When do configuration for redis non-cluster session manager. please use below pair.
<Valve className="com.orangefunction.tomcat.redissessions.RedisSessionHandlerValve" />
<Manager className="com.orangefunction.tomcat.redissessions.RedisSessionManager" "..."/>

when do configuration for redis cluster session manager, please use below pair.
<Valve className="com.orangefunction.tomcat.redissessions.RedisClusterSessionHandlerValve" />
<Manager className="com.orangefunction.tomcat.redissessions.RedisClusterSessionManager" "..."/>

for more configuraion details, please refer below.

Reference for redis cluster approache
[https://github.com/zhmz1326/tomcat-redis-session-manager.git]

Reference of original approach
[https://github.com/jcoleman/tomcat-redis-session-manager.git]


Please note - This version is only tested in some limited area. So please take into consideration before introduce it into PRODUCTION environment.  

And also, I'm very happy to know if you find any issue during your testing.

Br, 
(Bob) XuYong Hou
