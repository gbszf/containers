FROM biocontainers/biocontainers:vdebian-buster-backports_cv1
MAINTAINER biocontainers <biodocker@gmail.com>
LABEL    software="fitbit" \ 
    base_image="biocontainers/biocontainers:vdebian-buster-backports_cv1" \ 
    container="fitbit" \ 
    about.summary="FitBit REST API Client Implementation - Python 2" \ 
    about.home="https://github.com/orcasgit/python-fitbit/" \ 
    software.version="0.3.0-4-deb-py2" \ 
    upstream.version="0.3.0" \ 
    version="1" \ 
    about.copyright="(C) 2012-2017 ORCAS" \ 
    about.license="Apache-2.0" \ 
    about.license_file="/usr/share/doc/fitbit/copyright" \ 
    about.tags="devel::lang:python, devel::library, field::medicine, field::statistics,:python, role::devel-lib, science::data-acquisition" 

USER root
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update && (apt-get install -t buster-backports -y python-fitbit || apt-get install -y python-fitbit) && apt-get clean && apt-get purge && rm -rf /var/lib/apt/lists/* /tmp/*
USER biodocker
