FROM python:2.7
MAINTAINER Julien DAUPHANT

RUN apt-get update
RUN apt-get install -y python-opencv python-numpy xz-utils gifsicle 
RUN pip install youtube_dl
RUN pip install moviepy
RUN wget --quiet http://johnvansickle.com/ffmpeg/releases/ffmpeg-release-64bit-static.tar.xz && tar -xf ffmpeg-release-64bit-static.tar.xz && cp ffmpeg-*-64bit-static/ffmpeg /usr/local/bin/ && rm -rf ffmpeg-*-64bit-static ffmpeg-release-64bit-static.tar.xz
RUN ln /dev/null /dev/raw1394
ENV IMAGEIO_FFMPEG_EXE /usr/local/bin/ffmpeg 
