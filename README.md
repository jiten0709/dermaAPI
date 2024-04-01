
# DERMALYSE APP'S API

This API call is used to detect what top 3 most probable diseases a provided image is.
Its a made with Flask framework...follow SETUP STPES to locally run it on your machine.

## API Reference

#### Send image as payload

```http
  POST /5000:predict/
```

```http
  Response {'disease1': probability1,'disease2': probability2,'disease3': probability3}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `file` | `base64 encoded` | **Required**. an image file converted to base64 encoded|



## Run Locally

Clone the project

```bash
  git clone https://github.com/jiten0709/dermaAPI.git
```

Go to the project directory

```bash
  cd dermaAPI
```

Create a VirtualEnv

```bash
python3.10 -m venv my_venv
```

Activate VirtualEnv

```bash
source my_venv/bin/activate
```

Install dependencies

```bash
  pip install -r requirements.txt
```

Start the server

```bash
  python3 main.py
```

