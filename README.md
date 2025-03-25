# 🐳 WordPress + MySQL Docker Compose Setup

Easily deploy WordPress with MySQL using Docker Compose. This repository provides a ready-to-use docker-compose.yml file to spin up a WordPress site in minutes.

## 📂 Project Structure
```htm
.
├── docker-compose.yml    # Docker Compose configuration
└── README.md             # Documentation
```

## 🚀 Quick Start

Ensure you have Docker and Docker Compose installed on your system.

1. Clone the Repository
```json
git clone https://github.com/your-username/wordpress-docker-compose.git
cd wordpress-docker-compose
```

2. Start the Containers
```json
docker-compose up -d
```

3. Access WordPress

Open your browser and navigate to:
```json
# http://<IP Addr>:8080
http://192.168.10.152:8080
```

4. Stop the Containers
```json
docker-compose down
```


## 📊 Environment Variables

| Variable              | Description                          | Default Value             |
|-----------------------|--------------------------------------|---------------------------|
| `WORDPRESS_DB_HOST`   | MySQL database hostname              | `db`                      |
| `WORDPRESS_DB_USER`   | WordPress database username          | `wordpress`               |
| `WORDPRESS_DB_PASSWORD`| WordPress database password          | `wordpress`               |
| `WORDPRESS_DB_NAME`   | WordPress database name              | `wordpress`               |
| `WP_HOME`             | Public URL for WordPress site        | `http://192.168.10.152:8080` |
| `WP_SITEURL`          | WordPress installation URL           | `http://192.168.10.152:8080` |


## 📦 Data Persistence

The WordPress site and MySQL database are stored in Docker volumes:
- wordpress_data – Stores WordPress files
- db_data – Stores MySQL data

## 🔍 Troubleshooting
1. Ensure Docker and Docker Compose are installed and running.
2. Verify the IP address (192.168.10.152) is correct and accessible from other devices.
3. Check logs for errors:
```json
docker-compose logs -f
```
## 🤝 Contributing

Feel free to fork this repository, open issues, or submit pull requests!

## 📜 License

This project is licensed under the MIT License.

