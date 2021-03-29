FROM kienkauko/ubuntu:gnu
COPY . /home/
WORKDIR /home/
RUN gcc server.c -o server
CMD ["./server"]
EXPOSE 8080
