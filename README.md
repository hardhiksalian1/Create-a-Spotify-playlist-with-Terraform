# Create-a-Spotify-playlist-with-Terraform
Use a Terraform data source to search Spotify for an artist, album, or song, and use that data to build a playlist.

Pre Requisite:

- docker desktop
- spotify dev account (refer- " https://developer.hashicorp.com/terraform/tutorials/community-providers/spotify-playlist ")
- terraform
- VS code

* create .env file in same folder as project to store your Spotify application's client ID and secret.
* run docker in terminal with this command : docker run --rm -it -p 27228:27228 --env-file .env ghcr.io/conradludgate/spotify-auth-proxy
  - API_KEY will generate in this command
  - in AUTH url link click on accept

commands :
- terraform init (terraform.tfstate file will be generated)
- terraform plan
- terraform apply -auto-approve
(do this in seperate terminal as docker container needs to be running in other terminal)
