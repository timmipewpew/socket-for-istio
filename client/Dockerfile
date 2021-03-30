FROM kienkauko/ubuntu:gnu
COPY . /home/
WORKDIR /home/
RUN make
CMD ["./client"]
EXPOSE 8080
RUN apt-get install -y netcat
RUN nc -l -p 8080
RUN nc sp-server 8080
