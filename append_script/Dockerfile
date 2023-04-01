FROM alpine:3

WORKDIR /app/

COPY . .

RUN chmod +x input_site.sh

CMD [ "./input_site.sh" ]

# run with `docker run -it --name a_name <image_name> sh` 
# to avoid exec format error
