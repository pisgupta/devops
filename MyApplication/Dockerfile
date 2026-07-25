# Use official Gradle + JDK image
FROM gradle:8.7.0-jdk17 AS build

# Set working directory
WORKDIR /app

# Copy project files
COPY . .

# Run Gradle build (assembleDebug or assembleRelease)
RUN gradle assembleDebug