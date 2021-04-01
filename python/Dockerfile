FROM python:slim

RUN pip install --no-cache-dir notebook bash_kernel

RUN python -m bash_kernel.install

ENTRYPOINT ["/usr/local/bin/jupyter", "notebook", "--allow-root", "--no-browser"]
CMD ["--ip='*'", "--port=8888", "--notebook-dir=/root"]
