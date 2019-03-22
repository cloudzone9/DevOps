    FROM store/oracle/database-instantclient:12.2.0.1
    RUN curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
    RUN python get-pip.py
    WORKDIR /Python_Application
    ADD . /Python_Application
    RUN pip install -r req.txt
    EXPOSE 5000
    CMD ["python","./Fusion/common/rest_server.py"]