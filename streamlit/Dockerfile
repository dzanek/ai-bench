FROM python:3.10

COPY . /app
# Set the working directory
WORKDIR /app


# Install the required packages
RUN pip install streamlit


# Expose the port Streamlit will run on
EXPOSE 8501

# Use ENTRYPOINT for the main command
ENTRYPOINT ["streamlit", "run", "app.py", "--server.port=8501"]
