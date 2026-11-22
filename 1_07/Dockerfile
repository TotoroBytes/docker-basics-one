# Start from the ubuntu image
FROM ubuntu:24.04

RUN apt-get update && apt-get install -y curl

# Copy the hello.sh file from this location to /usr/src/app/ creating /usr/src/app/hello.sh.
COPY script.sh .

# When running Docker run the command will be ./hello.sh
ENTRYPOINT ["./script.sh"]
