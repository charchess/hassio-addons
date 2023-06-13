FROM codeproject/ai-server:gpu

ARG TZ=Europe/Paris

VOLUME ["/data"]

# Define default environment variables
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fix a memory leak on encoded recording
ENV MALLOC_TRIM_THRESHOLD_=100000

# Main UI port
EXPOSE 32168

ENTRYPOINT ["./CodeProject.AI.Server"]
LABEL \
  io.hass.version="VERSION" \
  io.hass.type="addon" \
  io.hass.arch="amd64"