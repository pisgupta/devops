# Use official Gradle + JDK image
#FROM gradle:9.4.1-jdk17 AS build

# Set working directory
#WORKDIR /app

# Copy project files
#COPY . .

# Run Gradle build (assembleDebug or assembleRelease)
#RUN gradle assembleDebug

# Use an image that already has Android SDK, Java, and Gradle installed
FROM thyrlian/android-sdk:latest

# Set working directory inside container
WORKDIR /app

# Copy your project files into the container
COPY . .

# Give execution permission to the gradlew script
RUN chmod +x ./gradlew

# Now run the build
RUN ./gradlew assembleDebug