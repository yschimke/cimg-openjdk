# vim:set ft=dockerfile:

FROM cimg/base:2020.03

LABEL maintainer="Community & Partner Engineering Team <community-partner@circleci.com>"

ENV JAVA_VERSION 8.0.252
ENV URL https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u252b09.tar.gz
ENV JAVA_HOME /usr/local/jdk-${JAVA_VERSION}

RUN curl -sSL -o java.tar.gz "${URL}" && \
        sudo mkdir /usr/local/jdk-${JAVA_VERSION} && \
        sudo tar -xzf java.tar.gz --strip-components=1 -C /usr/local/jdk-${JAVA_VERSION} && \
        rm java.tar.gz && \
        $JAVA_HOME/bin/java -version && $JAVA_HOME/bin/javac -version

ENV JAVA_VERSION 8.0.242
ENV URL https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u242b08.tar.gz
ENV JAVA_HOME /usr/local/jdk-${JAVA_VERSION}

RUN curl -sSL -o java.tar.gz "${URL}" && \
        sudo mkdir /usr/local/jdk-${JAVA_VERSION} && \
        sudo tar -xzf java.tar.gz --strip-components=1 -C /usr/local/jdk-${JAVA_VERSION} && \
        rm java.tar.gz && \
        $JAVA_HOME/bin/java -version && $JAVA_HOME/bin/javac -version

ENV JAVA_VERSION 14.0.1
ENV URL https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.1%2B7/OpenJDK14U-jdk_x64_linux_hotspot_14.0.1_7.tar.gz
ENV JAVA_HOME /usr/local/jdk-${JAVA_VERSION}

RUN curl -sSL -o java.tar.gz "${URL}" && \
	sudo mkdir /usr/local/jdk-${JAVA_VERSION} && \
	sudo tar -xzf java.tar.gz --strip-components=1 -C /usr/local/jdk-${JAVA_VERSION} && \
	rm java.tar.gz && \
        $JAVA_HOME/bin/java --version && $JAVA_HOME/bin/javac --version

ENV JAVA_VERSION 11.0.7
ENV URL https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.7_10.tar.gz
ENV JAVA_HOME /usr/local/jdk-${JAVA_VERSION}

RUN curl -sSL -o java.tar.gz "${URL}" && \
        sudo mkdir /usr/local/jdk-${JAVA_VERSION} && \
        sudo tar -xzf java.tar.gz --strip-components=1 -C /usr/local/jdk-${JAVA_VERSION} && \
        rm java.tar.gz && \
        $JAVA_HOME/bin/java --version && $JAVA_HOME/bin/javac --version

