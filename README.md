## PHP-Reaper - PHP tool to scan ADOdb code for SQL Injections
[![Docker Pulls](https://img.shields.io/docker/pulls/rvannauker/php-reaper.svg)](https://hub.docker.com/r/rvannauker/php-reaper/) [![Docker Stars](https://img.shields.io/docker/stars/rvannauker/php-reaper.svg)](https://hub.docker.com/r/rvannauker/php-reaper/) [![](https://images.microbadger.com/badges/image/rvannauker/php-reaper:latest.svg)](https://microbadger.com/images/rvannauker/php-reaper:latest) [![GitHub issues](https://img.shields.io/github/issues/RichVRed/docker-php-reaper.svg)](https://github.com/RichVRed/docker-php-reaper) [![license](https://img.shields.io/github/license/RichVRed/docker-php-reaper.svg)](https://tldrlegal.com/license/mit-license)

Docker container to install and run php-reaper

### Installation / Usage
1. Install the rvannauker/php-reaper container:
```bash
docker pull rvannauker/php-reaper
```
2. Run php-reaper through the php-reaper container:
```bash
sudo docker run --rm --volume $(pwd):/workspace --name="php-reaper" "rvannauker/php-reaper" -d {destination}
```

### Download the source:
To run, test and develop the PHP-REAPER Dockerfile itself, you must use the source directly:
1. Download the source:
```bash
git clone https://github.com/RichVRed/docker-php-reaper.git
```
2. Build the container:
```bash
sudo docker build --force-rm --tag "rvannauker/php-reaper" --file php-reaper.dockerfile .
```
3. Test running the container:
```bash
 $ docker run rvannauker/php-reaper --help
```