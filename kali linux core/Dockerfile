FROM kalilinux/kali-rolling

MAINTAINER [AT]aguztynbassi

# init
ENV DEBIAN_FRONTEND noninteractive
ENV INITRD No

# Fix resolvconf issues with Docker
RUN echo "resolvconf resolvconf/linkify-resolvconf boolean false" | debconf-set-selections

# Term
ENV TERM xterm

# Ignore missing packages; if packages cannot be retrieved or fail the integrity check after retrieval (corrupted package files), hold back those packages and handle the result.
RUN apt-get update --fix-missing

# /etc/locale.gen This file lists locales that you wish to have built. You can find a list of valid supported locales at /usr/share/i18n/SUPPORTED. If /etc/locale.gen does not exist, create it.
RUN apt-get install -y locales && sed -i -e 's/\# es_AR.UTF-8 UTF-8/es_AR.UTF-8 UTF-8/g' /etc/locale.gen && locale-gen
ENV LANG es_AR.UTF-8
ENV LANGUAGE es_AR.UTF-8
ENV LC_ALL es_AR.UTF-8
ENV LC_CTYPE es_AR.UTF-8

# update and install packages
RUN apt-get -y upgrade && apt-get install -y kali-linux-core
