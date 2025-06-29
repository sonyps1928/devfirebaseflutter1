FROM cirrusci/flutter:beta

# Install Firebase CLI
RUN curl -sL https://firebase.tools | bash

# Optional Android SDK / Java setup
RUN apt-get update && apt-get install -y \
    openjdk-17-jdk adb wget unzip libglu1-mesa \
    && rm -rf /var/lib/apt/lists/*

ENV JAVA_HOME="/usr/lib/jvm/java-17-openjdk-amd64"
