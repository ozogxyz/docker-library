# MLflow Tracking server with MySQL as backend database for
# storing MLflow runs.
FROM python:3.7-slim-buster

# Set multiple labels at once, using line-continuation characters to break long lines
LABEL vendor=ACME\ Incorporated \
      com.ozogxyz.is-beta= "Yes"\
      com.ozogxyz.is-production="No" \
      com.ozogxyz.version="0.0.1-beta" \
      com.ozogxyz.release-date="21.11.2022"

# Cache busting
RUN apt-get update && apt-get install -y \
 && rm -rf /var/lib/apt/lists/*

# Run pip to install mlflow from req.txt
RUN pip3 install --no-cache-dir --user -r /req.txt


