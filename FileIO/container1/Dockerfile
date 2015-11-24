FROM ubuntu:14.04
RUN echo "Content Generated Inside Container1" > file.txt
RUN apt-get update && apt-get install -y socat
EXPOSE 9001
COPY ./start /
RUN chmod +x start
CMD ["/start"]


