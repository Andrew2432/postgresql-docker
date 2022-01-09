## PostgreSQL Docker

Steps to run PostgreSQL using Docker:

0. Make sure you have [Docker](https://www.docker.com/) and [Docker Compose](https://docs.docker.com/compose/) installed.
1. Clone the repository.
2. Create `data` folder inside the cloned repository.
3. - Copy the .env.example file into your choice of .env file (.env.development, .env.production etc.) . For our use, we prefer .env :
     ` cp .env.example .env`
   - Update `.env` based on your preferences.

4. Depending upon your `.env` file, make the changes in `up.sh` and `down.sh` files.
5. Create a separate network to run PostgreSQL and Adminer:
   ` sudo docker create network postgres_network`
6. - To start, `./up.sh`
   - To stop, `./down.sh`
