FROM python:slim

ENV http_proxy=http://195.221.0.35:8080
ENV https_proxy=http://195.221.0.35:8080
ENV ftp_proxy=http://195.221.0.35:8080

RUN pip install --no-cache-dir notebook bash_kernel

RUN python -m bash_kernel.install

ENTRYPOINT ["/usr/local/bin/jupyter", "notebook", "--allow-root", "--no-browser"]
CMD ["--ip='*'", "--port=8888", "--notebook-dir=/root"]
