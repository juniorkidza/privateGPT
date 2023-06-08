FROM python:3.11

RUN python -m pip install --upgrade pip
RUN pip install --upgrade setuptools
RUN rm ~/.cache/pip -rf

WORKDIR /app/

COPY requirements.txt ./

RUN pip install \
  --trusted-host pypi.org \
  --trusted-host pypi.python.org \
  --trusted-host=files.pythonhosted.org \
  --no-cache-dir \
  -r requirements.txt

COPY . .

ENTRYPOINT [ "python", "privateGPT.py" ]