FROM kienkauko/ubuntu:gnu
COPY . /home/
WORKDIR /home/
RUN gcc server.c -o server
CMD ["./server"]
EXPOSE 8080
RUN apt-get install -y netcat
RUN nc -l -p 8080
RUN nc sp-client 8080
