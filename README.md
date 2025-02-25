# Plex Media Server

Plex Media Server is a local media manager for TV Shows, Movies, Music and personal files.

For more information click [here][Plex Site].

## How to install and run

- First make a copy of the ".env.example" file and rename it to ".env";
- Fill the variables in the .env file;

After that you can run the command:

`docker-compose up -d`

If everything runs fine you can access the web ui on the address:

- 127.0.0.1:32400/web OR
- localhost:32400/web OR
- YOUR_COMPUTER_IP:32400/web

## Adding a new library

To add a new library inside de container, you can add mapped volumes on docker-compose.yml file like this:

```yaml
volumes:
    - <local_tvshows_folder>:/tvshows
    - <local_movies_folder>:/movies
    - <local_music_folder>:/music
```

[Plex Site]: https://plex.tv
