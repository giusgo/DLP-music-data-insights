<div align="center">

<img width="400px" src="./img/logo.png"></img>

</div>

<hr>

This repository aims to bring a bundle for the webapp. Both front-end and back-end have been dockerized to make it easy to run the applications.

<div align="center">

![](./img/demo.png)

</div>

## Project repositories

### Front-end
Visit the project [here](https://github.com/giusgo/DLP-frontend).

### Back-end
Visit the project [here](https://github.com/Torrex123/Spotify).

## Installation

Install [Docker](https://docs.docker.com/get-docker/).

Create a folder to keep both repositories and build the application:

```bash
mkdir 'DLP-music-data-insights' && cd 'DLP-music-data-insights'
```

Download the data from Kaggle [here](https://www.kaggle.com/datasets/mcfurland/10-m-beatport-tracks-spotify-audio-features) and place all the csv files under `csv_files` folder:

```bash
mkdir 'csv_files'
```

Clone both repositories (front-end and back-end):

```bash
git clone https://github.com/giusgo/DLP-frontend && git clone https://github.com/Torrex123/Spotify
```

Download the `docker-compose.yml` file in this repository:

```bash
wget https://raw.githubusercontent.com/giusgo/DLP-music-data-insights/main/docker-compose.yml
```

Build and run the application:

```bash
docker-compose up -d

# If using docker-compose-plugin
docker compose up -d
```

**NOTE:** Since all the data needs to be migrated from `.csv` format to a database, you need to wait a long time before using the webapp. 

Open your web browser and go to `http://ip_address:5044`. Where `ip_address` may be localhost or the IP address of the server you decide to host the app.
