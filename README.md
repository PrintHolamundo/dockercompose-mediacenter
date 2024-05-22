# 🎬 Docker Compose Project for a TV Show and Movie Library 🎥

This project uses Docker Compose to automate the creation and management of a TV show and movie library. Here is a description of each service and how they combine:

## 📂 Samba
Samba is used to share files over the network. In this project, it is used to share media and downloads.

## 🎵 Plex
Plex is a media server that organizes your collections of movies, TV shows, music, and photos and streams them to all your devices.

## ⬇️ Transmission
Transmission is a BitTorrent client used for downloading torrent files. In this project, it is used to download TV shows and movies.

## 📺 Sonarr
Sonarr is a TV show management application that will automatically search for new episodes of your favorite shows and download them.

## 🎞️ Radarr
Radarr is a movie management application that will automatically search for new movies you are interested in and download them.

## 🔍 Jackett
Jackett works as a proxy between the Sonarr, Radarr applications and various torrent trackers, allowing the search and download of torrents.

All these services combine to create an automated TV show and movie library. Torrent files are downloaded with Transmission, then Sonarr and Radarr automatically search and download the TV shows and movies you are interested in. Plex organizes and streams these media, and Samba allows sharing these files over the network.

## 🚀 How to run the project

To run this project you need to have Docker and Docker Compose installed. Then, you should configure the `.env` file with the paths to your media and storage directories.

Once you have configured the `.env` file, you can start all the services with the following command:

```bash
docker-compose up -d