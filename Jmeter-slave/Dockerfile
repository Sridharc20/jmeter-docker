#Server docker file should be inherited from the base image and should expose port 1099 and 50000. 
FROM sridharc20/jmbase
MAINTAINER Sridhar.C
# Ports to be exposed from the container for JMeter Slaves/Server
EXPOSE 1099 50000

# Application to run on starting the container
ENTRYPOINT $JMETER_HOME/bin/jmeter-server \
                        -Dserver.rmi.localport=50000 \
                        -Dserver_port=1099