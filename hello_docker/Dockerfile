# We can use alpine as our base image due to it being a pretty small 
# and lightweight linux distro. It won't have as many tools as a base
# Ubuntu image however. 
# We keep the image version locked with this specific tag to prevent us 
# auto updating into a breaking change
FROM alpine:3.13 

# Use /usr/src/app as our workdir. The following instructions will be  
# executed in this location.
WORKDIR /usr/src/app

# Copy the hello.sh file from this location to /usr/src/app/ creating /usr/src/app/hello.sh
COPY hello.sh .

# Alternatively, if we skipped chmod earlier, we can add execution permissions during the build.
RUN chmod +x hello.sh

# When running docker run the command will be ./hello.sh
# `.` denotes the working directory
CMD ./hello.sh

