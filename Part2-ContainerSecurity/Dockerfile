# Use a minimal base image
FROM alpine:3.12

# Add a non-root user
RUN addgroup -S appgroup && adduser -S ostafon -G appgroup

# Switch to the non-root user
USER ostafon

# Copy application files
COPY . /app

# Set the working directory
WORKDIR /app

# Run the application
CMD ["./app"]
