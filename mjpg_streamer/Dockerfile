FROM chuckleb/mjpg-streamer

RUN echo 'ls -la /dev/video0 && mjpg_streamer -o "output_http.so -w ./www -p 8081" -i "input_uvc.so mjpg_streamer -r VGA -f 10"' > /start.sh && chmod a+rx /start.sh

ENTRYPOINT /start.sh
