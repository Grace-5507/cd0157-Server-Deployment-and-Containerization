FROM  public.ecr.aws/sam/build-python3.7:latest

COPY . /app
WORKDIR /app

RUN pip install --upgrade pip
RUN pip install flask


ENTRYPOINT ["gunicorn", "-b", ":8080", "main:APP"]

