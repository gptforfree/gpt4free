FROM python:3.10-slim

RUN apt-get update && apt-get install -y git

RUN git clone https://github.com/xtekky/gpt4free.git
WORKDIR /gpt4free
RUN pip install --no-cache-dir -r requirements.txt
RUN pip install g4f
EXPOSE 8501

CMD ["python3", "g4f/gui/run.py"]