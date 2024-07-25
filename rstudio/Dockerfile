FROM --platform=linux/amd64 rocker/rstudio

RUN if [ -d "/etc/rstudio" ]; then \
        echo "www-frame-origin=same" >> /etc/rstudio/disable_auth_rserver.conf; \
    elif [ -d "/etc/rstudio-server" ]; then \
        echo "www-frame-origin=same" >> /etc/rstudio-server/disable_auth_rserver.conf; \
    else \
        echo "RStudio configuration directory not found"; \
        exit 1; \
    fi